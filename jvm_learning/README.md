# 编译 jvm
`
cd /Users/bytedance/infra/git/jdk8u/
bash ./configure --with-target-bits=64 --with-boot-jdk=/opt/java-se-8u41-ri --with-debug-level=slowdebug --enable-debug-symbols ZIP_DEBUGINFO_FILES=0
make all ZIP_DEBUGINFO_FILES=0
`
# 修改 jvm 代码，之后再编译
`
cd /Users/bytedance/infra/git/jdk8u/jvm_learning/
/Users/bytedance/infra/git/jdk8u/build/linux-x86_64-normal-server-slowdebug/jdk/bin/java Test
`
