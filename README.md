1. bundle install

2. bundle exec berks install

3. bundle exec berks upload

4. ./make-lumberjack-key.sh

5. knife data bag create lumberjack

6. knife data bag from file lumberjack bag.json

7. knife bootstrap ddg-cc.local --ssh-user mas --sudo --node-name elk-example

8. knife node edit elk-example

    "run_list": [
        "recipe[elkstack::java]",
        "recipe[elkstack::single]"
    ]

9. knife ssh name:elk-example "sudo chef-client" -x mas -a ipaddress

