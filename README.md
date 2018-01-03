# Bounty-Puppet-Master

Artoo is an Enterprise Saas provider for Banks and MFIs. This means a few things,
1. We need to manage infrastructure across multiple tenants.
2. Each client might have a slightly different requirements in terms of scaling, compliance, security.
3. Approvals before production changes, access restrictions etc.

We need some flexibility in terms of setting up our infrastructure. We need multiple environments and access restrictions.
Multiple environment layers we have defined are - Dev, QA, UAT, Staging, Production. We have 25 employees at Artoo, 12 of whom are engineers. Not all employees and engineers can be provided access to all environments.

How would you go about writing scripts (Python, Ruby, Perl, Bash, Zsh, etc..) to setup these environments.

Some sample use cases are,
1. Kaushik is the engineering manager he needs access to Dev, QA, UAT. But not the later ones.
2. Geloth is a Production support engineer and he only needs access to Production.
3. Shrivatsa is the Release engineer who needs access to UAT, Staging and Production.
4. All the other engineers will need access to Dev and QA.
5. The other employees do not need server access but require read access to MySQL.
6. What happens when a employee moves to a different role with different access restrictions.
7. How would you handle accounts for new employees or employees leaving Artoo.
