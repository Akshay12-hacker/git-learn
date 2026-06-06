STEP 4: GitHub Setup (NON-NEGOTIABLE)
Generate SSH key:
ssh-keygen -t ed25519 -C "your_email@example.com"


Press Enter for everything.

Start SSH agent:

eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519


Copy key:

cat ~/.ssh/id_ed25519.pub


➡️ Paste this key into GitHub → Settings → SSH & GPG Keys.

Test:

ssh -T git@github.com


If GitHub says “successfully authenticated” → continue.
