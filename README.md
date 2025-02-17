# <h2 align=center>0g-node Setup Guide by CryptoAirdropHindi</h2>


# 1. Source the Client Script:

This will download and execute the `client.sh` script.
```
source <(wget -O - https://raw.githubusercontent.com/CryptoAirdropHindi/CAH-0g-node/refs/heads/main/client.sh)
```

# 2. Create and Edit `envfile.env`:

You need to create an environment configuration file.
```
nano envfile.env
```

# 3. Edit the `Private Key`:

- Replace YOUR_PRIVATE_KEY in the file with your actual private key.
- Once done, save the file by pressing:
- CTRL + X to exit.
- Y to confirm the save.
- Enter to finalize.

4. Start the Node with Docker:
This will run the `0g-da-client` container with the configured environment file.
```
docker run -d --env-file envfile.env --name 0g-da-client -v ./run:/runtime -p 51001:51001 0g-da-client combined
```
# 5. Done!
Your node should now be up and running. You can monitor the logs or status via Docker commands.

# Useful Docker Commands:
- Check status of the container:
```
docker ps
```
- View logs
```
docker logs -f 0g-da-client
```
--------------------------------------------------------------------------------------------------------------------------

"Great, all set! If you have any questions, don’t hesitate to ask in our Telegram channel."
Or if you'd like something more friendly and engaging:
- Telegram - https://t.me/Crypto_airdropHM
- Youtube - https://www.youtube.com/@CryptoAirdropHindi6
