# CubeCoders AMP Template: Factorio with Mod Updater

This is a custom application template for [CubeCoders AMP](https://cubecoders.com/AMP) that extends the standard Factorio dedicated server template. 

It automatically integrates [factorio-mod-updater](https://github.com/dreamdenizen/factorio-mod-updater) directly into the server start sequence. Every time the server starts, it will:
1. Download the latest version of `mod_updater`
2. Scan the `mods` directory for out-of-date mods
3. Download and install any available mod updates
4. Start the Factorio server

It supports both **Linux** and **Windows** AMP instances.

## Installation

### Method 1: Connecting via GitHub (Recommended)
1. Open your AMP web interface and go to **Configuration -> Instance Deployment**.
2. Scroll down to **Template Repositories** and click Add.
3. Enter `dreamdenizen/amp-factorio-with-mod-updater:main`
4. Click **Fetch Latest**.
5. When creating a new instance, you can now select **Factorio with Mod Updater**.

## Requirements
- CubeCoders AMP v2.5.0.10 or later
- Ensure that the instance has outgoing internet access so it can reach the Factorio Mod Portal and GitHub Releases network.

## Troubleshooting

If you encounter `State: 3` when updating or fetching the template:
Make sure no files in the cloned template directory are locked. In AMP, you **cannot** update instances from a template while they are currently running. Ensure any running `Factorio with Mod Updater` instances are fully **Stopped** before clicking "Fetch Latest" or "Update Instances".

## License
Provided as-is for the AMP and Factorio communities. Factorio is a trademark of Wube Software. AMP is a trademark of CubeCoders Ltd.
