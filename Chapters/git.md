## Generating a new SSH key
1. Open windows PowerShell
2. Paste the text below, substituting in your work address.

```cmd
ssh-keygen -t ed25519 -C "your_email@example.com"
```

This creates a new SSH key, using the provided email as a label.

> Generating public/private algorithm key pair.

When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.

> Enter a file in which to save the key (/c/Users/you/.ssh/id_algorithm):[Press enter]

At the prompt, type a secure passphrase. For more information, see "Working with SSH key passphrases."

> Enter passphrase (empty for no passphrase): [Type a passphrase]
> Enter same passphrase again: [Type passphrase again]


## Adding your SSH key to the ssh-agent

1. Ensure the ssh-agent is running. You can use the "Auto-launching the ssh-agent" instructions in "Working with SSH key passphrases", or start it manually:

```cmd
# start the ssh-agent in the background
$ eval "$(ssh-agent -s)"
> Agent pid 59566
```
2. Add your SSH private key to the ssh-agent. If you created your key with a different name, or if you are adding an existing key that has a different name, replace id_ed25519 in the command with the name of your private key file.

``` cmd
ssh-add ~/.ssh/id_ed25519
```

3. Add the SSH key to your account on GitHub. For more information, see "Adding a new SSH key to your GitHub account."


## Adding a new SSH key to your GitHub account


1. Copy the SSH public key to your clipboard.

```cmd

clip < ~/.ssh/id_ed25519.pub

```
 2.  the upper-right corner of any page[https://bitbucket.org/account/settings/ssh-keys/], click your profile photo, then click Settings.


## Testing your SSH connection

1. Enter the following:
```cmd
$ ssh -T git@bitbuck.org
# Attempts to ssh to Bitbucket
```
2. Verify that the fingerprint in the message you see matches GitHub's RSA public key fingerprint. If it does, then type yes:

> Hi username! You've successfully authenticated, but GitHub does not
> provide shell access.


## Git Branching -Remote Branches

```cmd
git remote show
```

```cmd
git ls-remote
```

the [link](https://git-scm.com/book/en/v2/Git-Branching-Remote-Branches) to explain git branching and remote branching clearly