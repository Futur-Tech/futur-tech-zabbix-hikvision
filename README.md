# Zabbix Monitoring for Hikvision Cameras and NVR

This template allows you to monitor Hikvision cameras and NVR devices using Zabbix. 

## Usage

Once the template is installed and assigned to the hosts, Zabbix will start monitoring the following:

- Ping response: Checks if the device responds to ping requests.
- HTTP port open: Verifies if the HTTP port (usually port 80) is open.
- RTSP port open: Checks if the specified RTSP port is open. By default, the template uses the macro `{$HIKVISION.PORT.RTSP}` to define the port number.
- Hikvision server port open: Verifies if the specified Hikvision server port is open. By default, the template uses the macro `{$HIKVISION.PORT.SERVER}` to define the port number.
- Hikvision items from Zabbix official template

You should modify the macro `{$HIKVISION_ISAPI_HOST}`, `{$USER}` and `{$PASSWORD}` for the official Zabbix template.

## Compatibility

This template is designed for Zabbix Server 6.0 or later.
