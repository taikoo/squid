include ../../Make.properties

MOD_NAME = mod_active_compress.so

all:clean $(OBJS) 
	$(MOD_LINK) mod_active_compress.o  -o $(MOD_NAME)
	
install:
	cp -rf *.so ../$(MOD_DIR)

clean:
	rm -rf $(OBJS) *.so

uninstall:
	rm -rf /usr/local/squid/sbin/$(MOD_NAME)	

%.o:	%.c
	$(MOD_GCC) $< -o $@

