export OS_USERNAME=admin
export OS_PASSWORD=tester
export OS_AUTH_URL="http://127.0.0.1:35357/v2.0"
export OS_ENDPOINT="http://127.0.0.1:35357/v2.0"
export OS_TENANT_NAME=admin
java -cp target/scala-2.11/keystone-ltest-assembly-1.0.jar keystone_ltest.bsearch.BSearch "$@"  --rounds 1 --minRps 1 --duration 10 --out-dir /home/USERNAME_HERE/test_kong/keystone_full_deployment/keystone-ltest/outp/
