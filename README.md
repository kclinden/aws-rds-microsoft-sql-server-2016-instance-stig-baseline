# aws-rds-microsoft-sql-server-2016-instance-stig-baseline

InSpec profile to validate the secure configuration of AWS RDS Microsoft SQL Server 2016, against [DISA](https://iase.disa.mil/stigs/)'s **Microsoft SQL Server 2016 Instance Security Technical Implementation Guide (STIG) Version 2, Release 1**.

## Getting Started  
It is intended and recommended that InSpec run this profile from a __"runner"__ host (such as a DevOps orchestration server, an administrative management system, or a developer's workstation/laptop) against the target remotely over __winrm__.

__For the best security of the runner, always install on the runner the _latest version_ of InSpec and supporting Ruby language components.__ 

Latest versions and installation options are available at the [InSpec](http://inspec.io/) site.

## Running This Profile

    inspec exec https://github.com/mitre/aws-rds-microsoft-sql-server-2016-instance-stig-baseline/archive/master.tar.gz -t winrm://<hostip> --user '<admin-account>' --password=<password> --reporter cli json:<filename>.json

Runs this profile over winrm to the host at IP address <hostip> as a privileged user account (i.e., an account with administrative privileges), reporting results to both the command line interface (cli) and to a machine-readable JSON file. 
    
The following is an example of using this command. 

    inspec exec https://github.com/mitre/aws-rds-microsoft-sql-server-2016-instance-stig-baseline/archive/master.tar.gz -t winrm://$winhostip --user 'Administrator' --password=Pa55w0rd --reporter cli json:mssql-database-results.json

## License 

* This project is licensed under the terms of the [Apache 2.0 license](https://github.com/mitre/aws-rds-microsoft-sql-server-2016-instance-stig-baseline/blob/master/LICENSE.md).

### NOTICE  

DISA STIGs are published by DISA IASE, see: https://iase.disa.mil/Pages/privacy_policy.aspx   
