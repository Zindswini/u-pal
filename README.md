# U-Pal
My personal customization of ublue for desktop use. A mix of [Bazzite](https://github.com/ublue-os/bazzite/) and my own personal use case apps.

As with any ublue startingpoint, the customizations are in [recipe.yml](/recipe.yml) and in the scripts folder.

Swim upstream for more info!

## Verification

These images are signed with sisgstore's [cosign](https://docs.sigstore.dev/cosign/overview/). You can verify the signature by downloading the `cosign.pub` key from this repo and running the following command:

    cosign verify --key cosign.pub ghcr.io/ublue-os/startingpoint

If you're forking this repo, the uBlue website has [instructions](https://ublue.it/making-your-own/) for setting up signing properly.

## Install
To rebase an existing Silverblue/Kinoite installation to the latest build:

```
sudo rpm-ostree rebase ostree-unverified-registry:ghcr.io/zindswini/u-pal:latest
```