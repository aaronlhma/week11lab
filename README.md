# week11lab

# weather update script, service, and timer
The <i>weather_update</i> script, <i>weather.service</i> and <i>weather.timer</i> updates a file at designated filepath with the current weather forecast, intended to be used on Ubuntu

# Installation

## script
The <i>weather_update</i> script should be placed in the <i> $HOME/bin </i> directory, or wherever user scripts are being stored

## weather.service & weather.timer
The <i>weather.service</i> and <i>weather.timer</i> files should be placed in the <i> /etc/systemd/system </i> directory

# Configuration

## script
Within the <i>weather_update</i> script, the variable <b> WTTR_PATH </b> can be changed to wherever the user wants to keep the weather file that will be written to. By default, this is set to /home/vagrant/weather

## weather.service
Within the <i>weather.service</i> file, the <b>ExecStart=</b> line should be changed to wherever the script is being stored

## weather.timer
The <i>weather.timer</i> file can be changed in order to change the time between updates. The <b>OnUnitInactiveSec=</b> line determines how often the weather.service is ran. By default, this is set to hourly

# Usage
To access the weather information, the file contents can be output to the screen using "cat <i>path_to_filename</i>

