# Connect AnyPostMD on GitHub

## 1. Add SSH key (one time)

Open [GitHub → Settings → SSH keys](https://github.com/settings/keys) → **New SSH key**.

- **Title:** `Mac — anypost`
- **Key type:** Authentication Key
- **Key:** paste the line below (your public key)

```text
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIBsIcJx6muNnSNbkS9YZHY+4TB2I8CFAPD/mmhFwaqwy olegsavchin@anypost.md
```

Save. Then verify:

```bash
ssh -T git@github.com
```

You should see: `Hi <username>! You've successfully authenticated...`

## 2. Create the repo on GitHub

As org **AnyPostMD** (or your user):

1. [New repository](https://github.com/organizations/AnyPostMD/repositories/new) → name **`anypost`** → Public → **no** README/license (we already have them)
2. Set **Website** to `https://anypost.md`
3. Topics: `markdown`, `llm`, `agents`, `webmcp`, `social-media`

## 3. Push from this folder

```bash
cd /Users/olegsavchin/Documents/anypost_github
git remote add origin git@github.com:AnyPostMD/anypost.git
git push -u origin main
```

## 4. Org profile README (optional)

Create repo **`AnyPostMD`** (same name as the org) and push `profile-README.md` from `anypost/docs/github/AnyPostMD/` as its `README.md`.

## 5. Pin + avatar

- Pin **anypost** on [github.com/AnyPostMD](https://github.com/AnyPostMD)
- Org avatar: use `static/logo.png` from this repo
