# MTConnect-Agent-Stylesheet
XML Stylesheet for MTConnect Agents using [Bootstrap](http://getbootstrap.com/). This provides a better appearance than the default stylesheet and also adds links to run Probe, Current, and Sample requests.

## About

### PC
![[Agent Stylesheet PC] ](https://raw.githubusercontent.com/TrakHound/MTConnect-Agent-Stylesheet/master/images/pc.png)

### Mobile
![[Agent Stylesheet Mobile]](https://raw.githubusercontent.com/TrakHound/MTConnect-Agent-Stylesheet/master/images/mobile.png)

### File Size
Just over 300 KB. This Includes the necessary files for jquery, bootstrap, and the logo image.

## Installation
1. Download the latest [release](../../../MTConnect-Agent-Stylesheet/releases)
2. Unzip the contents into the "Styles" folder for the MTConnect Agent.
3. Edit the Agent's configuration file (ex. agent.cfg) to look for the stylesheets as shown below:

#### Agent.cfg

```
Files {
    styles {
        Path = ../styles
        Location = /styles/
    }
    Favicon {
        Path = ../styles/favicon.ico
        Location = /favicon.ico
    }
}

DevicesStyle { Location = /styles/Devices.xsl }

StreamsStyle { Location = /styles/Streams.xsl }

```

4. Restart Agent
5. Navigate to Agent's url to view

## Customization
This stylesheet is easily customizable using the Custom.css file. Customizations can include any overrides of the standard bootstrap styles such as changing the colors of the panel headers. The logo and link can be changed by editing the following lines in both Devices.xsl and Streams.xsl as shown below:

```xml

<a class="navbar-brand" style="padding: 5px 20px;" href="http://www.mtconnect.org">
	<img alt="Brand" src="/styles/MTConnect-Logo.png" height="40"/>
</a>

```

## Contributions
Contributions to this project are welcome and please feel free to contact us directly at info@trakhound.com.

## License
This project is licensed under the MIT software license.




