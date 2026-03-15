Your "Pre-Flight" Checklist for each server:

    Capture the MAC:
        Find it on a sticker on the motherboard/chassis.
        Or, boot any Linux Live USB and run ip link show.
    Prep the recovery partition (eMMC or custom):
        Format it as ext4.
        Drop your setup-secrets.sh (passwords/SSH keys) onto it.
    Configure BIOS:
        Set UEFI Mode (disable Legacy/CSM).
        Set Boot Priority (USB > OS > Recovery)
        Disable Secure Boot (optional, but makes netbooting much smoother).
        Enable Power Recovery to Always On/Enabled
        Set the primary boot device (M.2 SDD or custom).
