- Dotnet core installation:
	- wget https://packages.microsoft.com/config/debian/11/packages-microsoft-prod.deb -O packages-microsoft-prod.deb && \
	  sudo apt install ./packages-microsoft-prod.deb && sudo apt-get update; \
	  sudo apt-get install -y apt-transport-https && \
	  sudo apt-get update && \
	  sudo apt-get install -y dotnet-sdk-7.0
- Solution for issue with network service delaying startup
	- network service delaying startup