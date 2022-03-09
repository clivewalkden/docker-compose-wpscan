# WP Scan in docker-compose

### Setup
Create a `.env` file from the `.env.sample` and add your WP Scan API Key.

### Usage
Using the convenient bash wrapper you can use the command as if it was installed locally and it will fire up a container and run the scan.

The output directory can be used to return your results back to the host machine if you include the `-o /wpscan/output/filename.ext` option.

`./wpscan --url 'https://www.example.com' --enumerate ap,at,tt,cb,dbe,u,m --output /wpscan/output/example.com.json --format json --ignore-main-redirect`