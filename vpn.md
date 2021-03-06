###How to establish new VPN connection with .ovpn configuration file (Ubuntu 14.04)

1. Execute the following commands in your Ubuntu terminal:
```
sudo apt-get install network-manager-vpnc openvpn network-manager-openvpn network-manager-openvpn-gnome
sudo /etc/init.d/networking restart
```

2. Open "Network Connections" window (VPN Connections -> Configure VPN)

3. Press "ADD" button, click on drop-down menu and pick "Import a saved VPN configuration", press Create button.

4. In "Select File to import" choose your "*.ovpn" file.

5. In "Editing ...your *.ovpn file name..." window enter your username and password for vpn. Make sure that a *.crt file appeared in CA Certificate field.

6. Open "IPv4 Settings" panel and choose "Automatic (VPN) addresses only".

7. Open "VPN" panel again and click "Advanced" button.

8. Open "TLS Authentication" panel and make sure your "*.key" appeared in "Key File" field. Press Ok button.

9. Press "Save" button in "Editing ...your *.ovpn file name..." window.

10. Your VPN connection should appear in "Network Connections" window.
