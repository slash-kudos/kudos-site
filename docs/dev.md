# Developer Docs

These docs have technical information about how to do developer stuff or how something was done manually in case we need to fix it in the future.

## Quick Reference

- [Manage slashkudos.com on Namecheap]
- [SiteGround Site Tools for slashkudos.com]

## Setup SiteGround

1. Go to https://my.siteground.com/websites/list
2. New Website
3. Existing Domain (if you already bought the domain on Namecheap)
4. Follow prompts for Wordpress. You can also skip and install Wordpress from Site Tools.

## Route to Wordpress on SiteGround using AWS Route 53

1. Update Namecheap to use AWS Route 53 DNS
  - ![Namecheap AWS Custom DNS Example](/docs/assets/namecheap-aws-dns-example.png)
2. Update AWS DNS to point to SiteGround
  1. Go to the DNS Zone Editor in Site Tools and copy all the DNS Records to Route 53. Don't copy MX and TXT. Just A records really. Copy the main domain A record first and reference the "alias to another record in this hosted zone" for the other records in Route 53.
  - ![AWS Route 53 Records](/docs/assets/aws-route53-records.png)
3. You can use the free "Let's Encrypt" SSL cert from SiteGround and enforce HTTPS

## Setup Emails for the new Domain

I already have a google workspace. So I can just add the new domain as a trusted domain to it, and then add an alias for my new email with the new domain.

1. Go to the [admin console](https://admin.google.com/)
1. [Add a domain](https://admin.google.com/ac/domains/manage)
1. Make it a secondary 
1. Follow the steps
1. Then Activate Gmail
1. Follow the steps
1. Then go to the Directory > Users
1. Add an alternate email
1. User the new domain

### Emails created for slashkudos.com

- philip@slashkudos.com

<!-- Links -->
[Manage slashkudos.com on Namecheap]: https://ap.www.namecheap.com/domains/domaincontrolpanel/slashkudos.com/domain
[SiteGround Site Tools for slashkudos.com]: https://tools.siteground.com/dashboard?siteId=S3czeFlYNFBJdz09
