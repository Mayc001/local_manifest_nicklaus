# local_manifest_nicklausLineageOS 14.1 para dispositivo Moto E4 Plus
Motorola Moto E4 Plus

Criar diretórios

	$ mkdir los-14.1
	$ cd los-14.1
os manifestos locais:

	# repo init -u git://github.com/LineageOS/android.git -b cm-14.1
	# git clone https://github.com/Mayc001/local_manifest_nicklaus.git -b los-14.1 .repo/local_manifests
Em seguida, sincronize com este comando:

	# repo sync -c -j16 --force-sync --no-clone-bundle --no-tags -q      ##( this is a silent sync )
Construindo a partir da fonte
	$ cd device/motorola/nicklaus/patches
	$ ./check-patches.sh
	$ ./apply-patches.sh
	$ . build/envsetup.sh
	$ lunch lineage_nicklaus-userdebug
	$ brunch nicklaus
Créditos:
@ darklord4822
@olegsvs
@MediatekAndroidDevelopers
@iykequame
@CarlosArriagaCM
@ SamarV-121
@ ashwinr64
igor1144
Decker
danielhk
mdeejay
Zormax
@Mohamed_Zumair
@Reblion
@ Manjunath-yashu
e mais pessoas: D
