# tmuxLoggingSetup
A pair of scripts intended to quickly set up logging capabilities for Tmux utilizing Tmux Plugin Manager (https://github.com/tmux-plugins/tpm)
Additionally, the continuum plugin is added to save and recover tmux sessions across reboots (https://github.com/tmux-plugins/tmux-continuum)

### Install
`git clone https://github.com/6sp33d/tmuxConfigSetup.git`

`cd tmuxConfigSetup && chmod +x installer.sh setup.sh`

`./installer.sh`

`tmux new -s abc`

```
# Within the tmux session source the new plugins.
Press: Prefix_key + I
```

`./setup.sh`

```
# Source the plugins 1 more time: 
Press: Prefix_key + I
```

Finished! Now in a tmux session we can do the following:

Description|Command
-|- 
Toggle logging on/off for the attached pane|`prefix + P`
Capture visable history for the attached pane|`prefix + k`
Capture full history (based on history-limit) for the attached pane|`prefix + l`
Clear history|`prefix + L`

**If you enable logging, the log file is written out when toggling is toggled off.*
