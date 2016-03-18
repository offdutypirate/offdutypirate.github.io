Title: SELinux Permissive Domains  
Date: 2016-03-18 12:05
Modified: 2016-03-18 12:05
Category: short tips
Slug: selinux-permissive-domains
Authors: Jon Moore

When SELinux is configured to run in Permissive mode it will only log when an action would be denied using Enforcing.  Using permissive domains a single process and be configured to run in Permissive mode while leaving the rest of the system in Enforcing.

Make a domain permissive with `semanage permissive *domain*`.  To remove a domain from the permissive list use `semanage permissive -d *domain*`.
