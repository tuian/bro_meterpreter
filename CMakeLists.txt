
cmake_minimum_required(VERSION 2.8)

project(Plugin)

include(BroPlugin)

bro_plugin_begin(NCSA Meterpreter)
bro_plugin_cc(src/Plugin.cc)
bro_plugin_bif(src/meterpreter.bif)
bro_plugin_dist_files(README CHANGES COPYING VERSION)
bro_plugin_end()
