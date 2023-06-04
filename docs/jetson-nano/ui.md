# Enable / Disable UI in Jetson Nano

By default the UI is enabled in Jetson Nano.

To disable GUI on boot, run:

```sh
sudo systemctl set-default multi-user.target
```

To enable GUI again issue the command:

```sh
sudo systemctl set-default graphical.target
```

To start Gui session on a system without a current GUI just execute:

```sh
sudo systemctl start gdm3.service
```

Then reboot

```sh
sudo reboot
```
