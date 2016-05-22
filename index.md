---
layout: default
---

## About
Codenize.tools manege any services by DSL.

For example, It is possible to manage the [Route53](http://aws.amazon.com/route53/) by the following Ruby code:

{% highlight ruby %}
hosted_zone "example.com." do
  rrset "example.com.", "A" do
    ttl 300
    resource_records(
      "127.0.0.1",
      "127.0.0.2"
    )
  end
end
{% endhighlight %}

## Why?
* Idempotency. The service is set according to the definition of code.
* It is easy to [grep](http://linuxcommand.org/man_pages/grep1.html) the service configuration.
* The service configuration can be managed by VCS.

## Tools

### AWS
- [Roadworker](https://github.com/roadworker) - Route53
- [Piculet](https://github.com/piculet) - Security Groups
- [Kelbim](https://github.com/kelbim) - ELB
- [Miam](https://github.com/miam) - IAM
- [Kumogata2](https://github.com/kumogata2) - CloudFormation
  - old version: [Kumogata](https://github.com/kumogata)
- [Eipmap](https://github.com/eipmap) - Elastic IP
- [Radiosonde](https://github.com/radiosonde) - CloudWatch Alarm
- [Meteorlog](https://github.com/meteorlog) - CloudWatch Logs
- [Mappru](https://github.com/winebarrel/mappru) - VPC Route table
- [Bukelatta](https://github.com/winebarrel/bukelatta) - S3 Bucket Policy
- [Repol](https://github.com/winebarrel/bukelatta) - ECR Repository Policy
- [Cfdef](https://github.com/winebarrel/cfdef) - CloudFront

### Other Service
- [Ridgepole](https://github.com/ridgepole) - DB(Rails)
- [Gratan](https://github.com/gratan) - MySQL privileges
- [Posgra](https://github.com/winebarrel/posgra) - PostgreSQL privileges
- [watch_list](https://github.com/watch_list) - Uptime Robot
- [Cronicle](https://github.com/cronicle) - Job Runner / Job Scheduler
- [Barkdog](https://github.com/winebarrel/barkdog) - Datadog monitors
- [Lbrt](https://github.com/winebarrel/lbrt) - Librato
