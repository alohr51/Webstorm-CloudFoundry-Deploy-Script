### Getting Started

##### Prerequisite

* Your Application directory must have a manifest.yml
  * Read more [here](https://docs.cloudfoundry.org/devguide/deploy-apps/manifest.html#minimal-manifest)

##### Steps

1. In WebStorm: File -> Settings -> Tools -> External Tools
1. Click the green `+` symbol
1. Name the tool
1. In **Program** provide the file path for `webstormCloudFoundryDeploy.bat`
1. In **Paramters** paste: `$Prompt$`
1. In **Working directory** paste: `$ProjectFileDir$`
1. To run the tool - In the top menu: Tools -> External Tools -> Whatever you named the tool
1. For the prompt you enter your credentials in this order with a space between them:
    * `<cf api target> <cf username> <cf password> <cf org name> <cf space name>`
    * **Order Matters**

#### Tips

* You do not have to keep entering the parameters if you use the **rerun** button on the terminal in WebStorm.
