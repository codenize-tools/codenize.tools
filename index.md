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
* It is easy to grasp the service configuration.
* The service configuration can be managed by VCS.

## Tools

### AWS
- [Roadworker](http://roadworker.codenize.tools/) - Route53
- [Piculet](http://piculet.codenize.tools/) - Security Groups
- [Kelbim](http://kelbim.codenize.tools/) - ELB
- [Miam](http://miam.codenize.tools/) - IAM
- [Kumogata](http://kumogata.codenize.tools/) - CloudFormation
- [Eipmap](http://eipmap.codenize.tools/) - Elastic IP
- [Radiosonde](http://radiosonde.codenize.tools/) - CloudWatch Alarm
- [Meteorlog](http://meteorlog.codenize.tools/) - CloudWatch Logs

### Other
- [Ridgepole](http://ridgepole.codenize.tools/) - DB(Rails)
- [Gratan](http://gratan.codenize.tools/) - MySQL permissions
- [watch_list](http://watch_list.codenize.tools/) - Uptime Robot
- [Cronicle](http://cronicle.codenize.tools/)
