# Chef

## Setting up a Chef server

    http://downloads.chef.io/chef-server/ubuntu/#/

    sudo chef-server-ctl reconfigure

    sudo chef-server-ctl user-create user_name first_name last_name email password --filename FILE_NAME

    sudo chef-server-ctl user-create stevedanno Steve Danno steved@chef.io abc123 --filename /path/to/file.key

    sudo chef-server-ctl org-create short_name full_organization_name --association_user user_name --filename FILE_NAME

    sudo chef-server-ctl org-create chef Chef Software, Inc. --association_user stevedanno --filename /path/to/file.key

    sudo chef-server-ctl install opscode-manage

    sudo opscode-manage-ctl reconfigure

    sudo chef-server-ctl reconfigure




## Bootstrapping a new node

    knife cookbook site download learn_chef_apache2

    # Remote server to bootstrap
    export ADDRESS=

    # Remote user to ssh as
    export USER=

    # Remote password
    export PASSWORd=

    export NODE_NAME=

    knife bootstrap $ADDRESS --ssh-user $USER --ssh-password $PASSWORD \
    --sudo --use-sudo-password --node-name $NODE_NAME \
    --run-list 'recipe[learn_chef_apache2]'
