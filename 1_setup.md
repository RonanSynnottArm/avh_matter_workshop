Setup Arm Virtual Hardware instances of Raspberry Pi 4.
---
## Login to your Arm Virtual Hardware console

Open your browser, and navigate to Arm Virtual Hardware console:
```console
https://app.avh.arm.com/
```
## Create Raspberry Pi 4 virtual devices

Click on `Create Device`.

Select `Raspberry Pi 4` from the list of available devices.

Select `Raspberry Pi OS lite` from the example firmware packages pulldown.

Name the device `chip-tool`, (please use exactly `chip-tool`, as this will be used later in the session), and create device. (advanced boot options etc can be ignored).

While this instance is being created, click `Devices` and repeat steps to create a second instance (suggest `lighting-app` as name).

Open each instance in its own browser pane. We shall use these browser panes throughout the workshop.

## Login to virtual Raspberry Pi instances

When your instances are created, select the `Console` tab, and log into each Raspberry Pi 4 instance.

* Username: `pi`
* Password: `raspberry`

It is also possible to log in via the CLCD window view. However it is easier to copy and paste (`Shift+Insert`) to the Console view.

### (Optional) Connect via SSH

The `Console` view within the browser will suffice for this workshop.

If you wish to connect to the instances via `SSH` (rather than `Console`), it is easiest to download and install the appropriate [OpenVPN Community](https://openvpn.net/community-downloads) version for your host.

In the Arm Virtual Hardware `Connect` tab, and scroll to the `Connect via VPN` section. Click on `DOWNLOAD OVPN FILE`.

In OpenVPN, select `Import` > `Import file...` and browse to the downloaded `OVPN FILE`. Click `Connect`.

On your host, open terminal(s), and connect to the virtual hardware instance(s) with the command shown in the `Connect` tab, or use your preferred terminal application.

## Install necessary software components

We shall build the Matter examples directly on the virtual Raspberry Pi 4 instances. To prepare for this, install the necessary dependencies on **each** instance. Your instances can be set up in parallel.

```console
sudo apt-get update
sudo apt-get install -y git gcc g++ python pkg-config libssl-dev libdbus-1-dev libglib2.0-dev libavahi-client-dev ninja-build python3-venv python3-dev python3-pip unzip libgirepository1.0-dev libcairo2-dev libreadline-dev
```
This will also verify that your instances are working correctly.

* [Proceed to next section -->](/2_build.md)
* [<-- Return to Workshop Home](/README.md)
