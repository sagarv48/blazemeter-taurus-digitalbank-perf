# blazemeter-taurus-digitalbank-perf
test-automation-in-practice with blazemeter,taurus and jmeter
 
Reference article: https://www.blazemeter.com/blog/test-automation-in-practice-a-tutorial

Docker commands:

docker pull digisic/digitalbank

docker run -p 8080:8080 digisic/digitalbank

docker run -it --rm --network="host" -v /home/vagrant/dev/files/taurus-blazemeter-demo/taurus-blazemeter-digitalbank:/bzt-configs -v /home/vagrant/dev/files/taurus-blazemeter-demo/taurus-blazemeter-digitalbank/my-run-artifacts:/tmp/artifacts blazemeter/taurus taurus-config.yaml
