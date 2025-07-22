cmake_minimum_required(VERSION 3.31)

find_package(cmake-pear REQUIRED PATHS node_modules/cmake-pear)

project(keet_appling C CXX ASM)

add_pear_appling(
  keet_appling
  ID keet
  NAME Keet
  VERSION 2.5.2
  AUTHOR Holepunch
  DESCRIPTION "Chat directly with your friends. Send messages, files, high quality videos and photos with no limitations. Private and Encrypted. Always Peer-to-Peer. Never on a server."

  MACOS_IDENTIFIER io.keet.app
  MACOS_CATEGORY public.app-category.developer-tools
  MACOS_ENTITLEMENTS
    com.apple.security.device.microphone
    com.apple.security.device.audio-input
    com.apple.security.device.camera
  MACOS_SIGNING_IDENTITY "09590CDE64938DA62FA174A68C240D346B05EF49"

  WINDOWS_SIGNING_SUBJECT "CN=Holepunch Inc, O=Holepunch Inc, S=British Virgin Islands (the), C=GB, OID.2.5.4.15=Private Organization, OID.1.3.6.1.4.1.311.60.2.1.2=British Virgin Islands (the), OID.1.3.6.1.4.1.311.60.2.1.3=GB, SERIALNUMBER=2009762"
  WINDOWS_SIGNING_THUMBPRINT "E890AF027C9C83F7427BCEEBE7AC533579DFE549"

  LINUX_CATEGORY AudioVideo
)
