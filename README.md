ec2-ssh
=======

SSH into EC2 instances via tag name

Changes
-------

This fork adds the following changes:

- Update ec2-host and ec2-ssh to read AWS credentials from ~/.ec2-ssh.conf.

Save your access key and secret keys in your ~/.ec2-ssh.conf to avoid having to set your AWS credentials in environment variables.

  [credentials]
  AWS_ACCESS_KEY_ID=[access_key]
  AWS_SECRET_ACCESS_KEY=[secret_key]

- Update ec2-ssh to add -i ID_FILE option for specifying ssh identity file

  $ ec2-ssh -i ~/.ssh/identity.pem 'Instance Tag'
