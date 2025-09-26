# Soundness-Testnet-Guide
<img width="1280" height="427" alt="image" src="https://github.com/user-attachments/assets/1afb72a3-8dc1-4129-9aea-5540e6df8fea" />
A command-line interface tool for interacting with Soundness Layer testnet.

# Testnet link:
https://soundness.xyz/blog/soundness-layer-testnet

# Install requirement
Using Docker MacBook, you can still try on window, open a new container and run the following commands

**Open Ubuntu shell**
```
docker run -it ubuntu

```
```
apt update
apt install curl git nano

```
```
apt update && apt install -y build-essential

```
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env

```
```
apt update && apt install -y pkg-config libssl-dev

```
```
apt-get update && apt-get install -y \
    build-essential \
    curl \
    pkg-config \
    libssl-dev
```
# Done with requirement, continue with soundness Setup

Paste the following Commands
```
curl -sSL https://raw.githubusercontent.com/soundnesslabs/soundness-layer/main/soundnessup/install | bash

```
```
source ~/.bashrc

```
```
soundnessup install

```
```
soundnessup update
```

# Generate a Key Pair
Generate a new key pair. Run the following command, replacing ``your-key-name`` with a name of your choice, watch the video below to know how to do that:

```
soundness-cli generate-key --name your-key-name
```


https://github.com/user-attachments/assets/46f4c421-2510-41eb-bb58-a5e4d28cab69

**Important**: A mnemonic phrase and Public Key will be displayed. Save it in a safe place! Store the key pair securely in a local ``key_store.json`` file, This is the only way to recover your key if it's lost.

# Importing a Key Pair
If you saved your mnemonic previously, you can import it to ``key_store.json`` by using following command:

```
soundness-cli import-key --name <name> --mnemonic "<mnemonic>"
```
Edit ``<name>`` to the name you used while generating it and Edit ``"<mnemonic>"`` to your mnemonic phrase

# Link Public Key to Discord
Go to discord https://discord.com/channels/1341336526713257984/1352604755712671814 Type /new_key send a place will pop up to input your new key then paste the new key send send

**NOTE:** Only for those with Onboarded role


# Open the Game Dashboard, Play the Game and Send Your Proof.

To play the game, go to Soundness Discord Server (link at the end of this page),then go to Game-Arena Channel.

Type /8queen in the text box and follow the onscreen instructions by clicking on the link in the bot response. It will take you to your browser.

play the game following the How to in the **8queen.txt** file of this repo.

<img width="540" height="906" alt="image" src="https://github.com/user-attachments/assets/67f048c8-eb7e-4b42-8528-99faf904a389" />

Once you have won the game, a ``Proof message will be Generated with your Blob ID included``, Copy it, edit ``<your-key-name>`` to the name you used when Generating key pair then submit your proof for verification via your CLI.

After completing everything the result will be like this
<img width="1049" height="583" alt="image" src="https://github.com/user-attachments/assets/5910e0e7-e781-43f1-a377-94584d750f5b" />


That's All

I'll make a video from beginning to the end on how to use this guide, check out my X(twitter), my dm is open for questions if you are confused

# Follow https://x.com/soundnesslabs and https://x.com/danieledekhe for updates

# Don't forget to fork and give a star ⭐