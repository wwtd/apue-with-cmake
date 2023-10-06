cmake_minimum_required(VERSION 3.5.1)
project(apue_cmake
        VERSION 0.0.1
        LANGUAGES C
        )

set(APUE_LIB_PATH "${PROJECT_SOURCE_DIR}/apue")
# message(${APUE_LIB_PATH})

add_library(apue STATIC 
            "${APUE_LIB_PATH}/lib/bufargs.c" 
            "${APUE_LIB_PATH}/lib/cliconn.c" 
            "${APUE_LIB_PATH}/lib/clrfl.c" 
            "${APUE_LIB_PATH}/lib/daemonize.c" 
            "${APUE_LIB_PATH}/lib/error.c" 
            "${APUE_LIB_PATH}/lib/errorlog.c" 
            "${APUE_LIB_PATH}/lib/lockreg.c" 
            "${APUE_LIB_PATH}/lib/locktest.c" 
            "${APUE_LIB_PATH}/lib/openmax.c" 
            "${APUE_LIB_PATH}/lib/pathalloc.c" 

            "${APUE_LIB_PATH}/lib/popen.c" 
            "${APUE_LIB_PATH}/lib/prexit.c" 
            "${APUE_LIB_PATH}/lib/prmask.c" 
            "${APUE_LIB_PATH}/lib/ptyfork.c" 
            "${APUE_LIB_PATH}/lib/ptyopen.c" 
            "${APUE_LIB_PATH}/lib/readn.c" 
            "${APUE_LIB_PATH}/lib/recvfd.c" 
            "${APUE_LIB_PATH}/lib/sendfd.c" 
            "${APUE_LIB_PATH}/lib/servaccept.c" 
            "${APUE_LIB_PATH}/lib/servlisten.c" 

            "${APUE_LIB_PATH}/lib/setfd.c" 
            "${APUE_LIB_PATH}/lib/setfl.c" 
            "${APUE_LIB_PATH}/lib/signal.c" 
            "${APUE_LIB_PATH}/lib/signalintr.c" 
            "${APUE_LIB_PATH}/lib/sleepus.c" 
            "${APUE_LIB_PATH}/lib/spipe.c" 
            "${APUE_LIB_PATH}/lib/tellwait.c" 
            "${APUE_LIB_PATH}/lib/ttymodes.c" 
            "${APUE_LIB_PATH}/lib/writen.c" 
            "${APUE_LIB_PATH}/lib/sleep.c" 
)
target_include_directories(apue PUBLIC "${APUE_LIB_PATH}/include")