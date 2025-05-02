Remove-NetFirewallRule -DisplayName "Allow IIS Port 8090" -ErrorAction SilentlyContinue
New-NetFirewallRule -DisplayName "Allow IIS Port 8090" -Direction Inbound -Protocol TCP -LocalPort 8090 -Action Allow -Profile Any
