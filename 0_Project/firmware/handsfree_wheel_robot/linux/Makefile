######################################define project name, board type, and path

#####ROBOT_MODEL : null mini stone stone_v2 stone_v3 stone_omni giraffe virtual
ROBOT_MODEL     ?= stone_v2
#####BOARD_TYPE: openre_board_mini openre_board_v2
BOARD_TYPE      ?= openre_board_v2
#####project name
PROJECT         =  robot_$(ROBOT_MODEL)_$(BOARD_TYPE)
TOP_PATH        =  ../../../..

#############################################################parameters

#####BOOTLOADER  : enable disable
BOOTLOADER_MODE ?= disable

##########################################################################source

CXX_SRC         += ../src/main.cpp 

#Includes
INCDIR          += -I. -I../src/ 

#########################################################################package

#PAKG: common robot_abstract math imu .....
PAKG        = common robot_abstract math imu motor sbus_ppm servo \
              robot_control hf_link tf
              
#OS_MODULE: UCOSII UCOSIII GUI FAT
OS_MODULE  =           

#LIB_MODULE: EIGEN MATRIX  etc
THIRDPARTY_MODULE = 

###################################################################include rules

include $(TOP_PATH)/0_Project/makefile/compiler.mk

