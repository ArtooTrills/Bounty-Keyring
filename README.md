# Bounty-Deployer
We want one click deploys, one-command deploys, git based.

### Setup
- Use this git repository as the base with 3 nodejs servers
- Use a Docker image or a VM as the deploy target.

### Instructions
- Use minimal off-the-shelf tooling.

#### Task
- On commit and push to remote a docker image / VM needs to be provisioned.
- Instead of a push you could also use a simple single command script.
- The whole repository or an archive can be copied over to remote machine.
- All the 3 NodeJS processes to be started on remote with a process monitoring tool like (foreverJS, PM2, SLC, ..)

### Analysis
- How did the remote server provisioning work. Does docker make this any easier?
- How did this differ from Dokku or Flynn.
- What did you learn doing this exercise.
- How would you do it if the 3 NodeJS services need to be deployed to 3 different remote hosts.

### Bonus
- If the NodeJS servers were talking to a database how would you provision the db?
- Create a simple UI where you can click to trigger the deployment.

### Final Words

When you are done, please just create a pull request on this repo. We would like you to come in and present your code to the whole team.

May the force be with you!

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
