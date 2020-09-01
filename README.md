# raspberry-pi-timelapse

Take a timelapse with a Raspberry Pi and Raspberry Pi Camera Module

Read the blog post on [cri.dev](https://cri.dev/posts/2020-09-01-Simple-Timelapse-with-a-Raspberry-Pi/#take-image-with-raspistill)

# Requirements

- Raspberry Pi + Camera Module

# Steps

1. Clone this repo on your Raspberry (`git clone https://github.com/christian-fei/raspberry-pi-timelapse.git`)
2. Enable Camera via `raspi-config` (in "Interfacing Options")
3. Add contents of the file `crontab` to your cron schedule via `crontab -e`
4. Generate a timelapse with e.g. `./create-timelapse 2020-09-01`

Optionally, to speed up timelapse creation on your PC

5. Clone this repo on your PC
6. `cp config.example.sh config.sh` and set up PI_USER and PI_HOST 
7. Sync snapshots with `./rsync-snapshots`
8. Generate a timelapse with e.g. `./create-timelapse 2020-09-01`
