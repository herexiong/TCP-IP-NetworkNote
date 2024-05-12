echo_src_c := echo_server.c echo_client.c
echo_obj := $(echo_src_c:.c=)

all: $(echo_obj)

$(echo_obj): %: %.c
	gcc $< -o $@

debug:
	@echo $(echo_obj)

clean:
	rm -f $(echo_obj)

.PHONY: all debug exec clean
