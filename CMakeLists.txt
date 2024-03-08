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

  WINDOWS_SIGNING_SUBJECT "<TODO>"
  WINDOWS_SIGNING_THUMBPRINT "<TODO>"

  LINUX_CATEGORY AudioVideo
)
