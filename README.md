# autorun
Execute scripts when connecting external drives (USB / eSATA) on a Synology NAS.

* DSM 7: [1.8](releases/tag/v1.8)
* DSM 6: [1.7](releases/tag/v1.7)
* DSM 5: [1.6](releases/tag/v1.7)
* older: [1.3](releases/tag/v1.3)


# install
Add https://www.cphub.net/ in the Package Center or manually install one from the [releases](releases).

Third Party packages are restricted by Synology in DSM 7. Since autorun does require root 
permission to perform its job an additional manual step is required after the installation.

SSH to your NAS (as an admin user) and execute the following command:

```shell
sudo cp /var/packages/autorun/conf/privilege.root /var/packages/autorun/conf/privilege
```


# build
Should run on any *nix box / subsystem.

* adjust the version number in INFO and build
* `./build`
* publish the created .spk

*Note that almost all of the UI is currently not included in the build (since I got bored of updating that with more or less every DSM version).*
