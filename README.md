# Ansible configuration for Django apps

#### Note: some configurations maybe harmful to your server, please read all the code with care

To set app-specific configs open `env_vars/base.yml` file and change the values to what suits your app

    server_name: DOMAIN_NAME
    app_name: APPLICATION_NAME
    repo_git_url: GIT_REPO_URL
    django_settings: DJANGO_SETTINGS_MODULE

Open `inventory` file to set your servers, IP's etc

and run playbook with code below

    $ ansible-playbook ansible/worker.yml -i ansible/inventory -e env=production