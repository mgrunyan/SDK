all: simpledemo threadeddemo threadedbatchdemo pollingdemo interleavingdemo twonetdemo compile

compile: compile.c
	$(CC) -o $@ $< -lm -lfwdnxt

simpledemo: simpledemo.c
	$(CC) -o $@ $< -lm -lfwdnxt

threadeddemo: threadeddemo.c
	$(CC) -o $@ -pthread $< -lm -lfwdnxt

threadedbatchdemo: threadedbatchdemo.c
	$(CC) -o $@ -pthread $< -lm -lfwdnxt

pollingdemo: pollingdemo.c
	$(CC) -o $@ $< -lm -lfwdnxt

interleavingdemo: interleavingdemo.c
	$(CC) -o $@ $< -lm -lfwdnxt

twonetdemo: twonetdemo.c
	$(CC) -o $@ $< $(CFLAGS) -lm -lfwdnxt

clean:
	rm -rf compile simpledemo threadeddemo threadedbatchdemo pollingdemo interleavingdemo twonetdemo

