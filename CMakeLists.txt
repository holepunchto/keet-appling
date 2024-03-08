cmake_minimum_required(VERSION 3.25)

project(pear_appling C)

include(pear)

add_pear_appling(
  pear_appling
  KEY keet
  NAME Keet
  VERSION 2.2.0
  AUTHOR Holepunch
  DESCRIPTION "Chat directly with your friends. Send messages, files, high quality videos and photos with no limitations. Private and Encrypted. Always Peer-to-Peer. Never on a server."

  MACOS_IDENTIFIER io.keet.app
  MACOS_CATEGORY public.app-category.developer-tools
  MACOS_ENTITLEMENTS
    com.apple.security.device.microphone
    com.apple.security.device.audio-input
    com.apple.security.device.camera
  MACOS_SIGNING_IDENTITY "09590CDE64938DA62FA174A68C240D346B05EF49"

  WINDOWS_SIGNING_SUBJECT "CN=Red Porridge With Creme ApS, O=Red Porridge With Creme ApS, S=Hovedstaden, C=DK, OID.2.5.4.15=Private Organization, OID.1.3.6.1.4.1.311.60.2.1.3=DK, SERIALNUMBER=37198625"
  WINDOWS_SIGNING_THUMBPRINT "C8303CD9273FA7147624B4821746FE4F9CB6E6CC"

  LINUX_CATEGORY AudioVideo
)
