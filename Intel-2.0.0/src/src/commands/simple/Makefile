# Makefile for commands/simple.

CFLAGS	= -D_MINIX -D_POSIX_SOURCE
CCLD	= $(CC) -i $(CFLAGS)
MAKE	= exec make -$(MAKEFLAGS) install

# This Makefile is large, but that is because it lists all actions that must
# be taken to compile and install all the simple commands.  If there were only
# one command then it would look like this:
#
# all:	bin \			need the 'bin' subdir
#	bin/cat \		need the 'bin/cat' executable
#
# bin:
#	mkdir bin		make the 'bin' subdir
#
# bin/cat:	cat.c		'bin/cat' is made from 'cat.c'
#	$(CCLD) -o $@ $?	compile 'cat.c' ($?) to 'bin/cat' ($@)
#	install -S 4kw $@	stack size is 8k (8086) or 16k (others)
#
# install:	bin \		rule to install all binaries
#	/usr/bin/cat \		one can find 'cat' in /usr/bin
#	/bin/cat \		important binaries are also in /bin
#
# /usr/bin/cat:	bin/cat
#	install -cs -o bin $? $@	copy 'bin/cat' to '/usr/bin/cat',
#					strip symbol table
#
# /bin/cat:	/usr/bin/cat
#	install -lcs $? $@	install '/bin/cat' by linking (if possible)
#				or copying (otherwise)
#
# Some of the binaries are installed under more than one name.  The extra
# names are indented by one extra tab in the install rule.
# If you want to add a command then insert it at the appropriate position
# in sorted order.  Search around for the command just above or below the
# the new command and add new rules for the new command near those places.
# Observe four key things:
#	What to make, how to make, what to install, how to install.

all:	bin \
	bin/add_route \
	bin/ascii \
	bin/at \
	bin/atrun \
	bin/backup \
	bin/badblocks \
	bin/banner \
	bin/basename \
	bin/btoa \
	bin/cal \
	bin/calendar \
	bin/cat \
	bin/cdiff \
	bin/cgrep \
	bin/chmem \
	bin/chmod \
	bin/chown \
	bin/ci \
	bin/cksum \
	bin/clr \
	bin/cmp \
	bin/co \
	bin/comm \
	bin/compress \
	bin/cp \
	bin/crc \
	bin/cron \
	bin/cut \
	bin/date \
	bin/dd \
	bin/decomp16 \
	bin/df \
	bin/dhrystone \
	bin/diff \
	bin/dirname \
	bin/diskcheck \
	bin/diskusage \
	bin/du \
	bin/dw \
	bin/echo \
	bin/ed \
	bin/eject \
	bin/expand \
	bin/expr \
	bin/factor \
	bin/fgrep \
	bin/file \
	bin/find \
	bin/finger \
	bin/fold \
	bin/fortune \
	bin/fsck \
	bin/fsck1 \
	bin/gather \
	bin/getty \
	bin/gomoku \
	bin/grep \
	bin/head \
	bin/host \
	bin/hostaddr \
	bin/id \
	bin/ifconfig \
	bin/ifdef \
	bin/in.fingerd \
	bin/in.rld \
	bin/in.rshd \
	bin/inodes \
	bin/install \
	bin/irdpd \
	bin/isoread \
	bin/join \
	bin/kill \
	bin/last \
	bin/leave \
	bin/life \
	bin/login \
	bin/look \
	bin/lp \
	bin/lpd \
	bin/ls \
	bin/mail \
	bin/man \
	bin/men \
	bin/mesg \
	bin/mkdir \
	bin/mkfifo \
	bin/mkfs \
	bin/mknod \
	bin/mkproto \
	bin/modem \
	bin/mount \
	bin/mref \
	bin/mt \
	bin/ncheck \
	bin/nm \
	bin/nonamed \
	bin/od \
	bin/passwd \
	bin/paste \
	bin/pathchk \
	bin/ping \
	bin/pr \
	bin/pr_routes \
	bin/prep \
	bin/pretty \
	bin/printenv \
	bin/printroot \
	bin/proto \
	bin/pwd \
	bin/pwdauth \
	bin/rarpd \
	bin/rcp \
	bin/readall \
	bin/readfs \
	bin/recover \
	bin/remsync \
	bin/rev \
	bin/rlogin \
	bin/rmdir \
	bin/roff \
	bin/rsh \
	bin/sed \
	bin/shar \
	bin/size \
	bin/sleep \
	bin/sort \
	bin/split \
	bin/strings \
	bin/strip \
	bin/stty \
	bin/su \
	bin/sum \
	bin/swapfs \
	bin/sync \
	bin/synctree \
	bin/tail \
	bin/tar \
	bin/tcpd \
	bin/tee \
	bin/term \
	bin/termcap \
	bin/test \
	bin/tget \
	bin/time \
	bin/touch \
	bin/tr \
	bin/traverse \
	bin/treecmp \
	bin/tsort \
	bin/ttt \
	bin/tty \
	bin/umount \
	bin/uname \
	bin/unexpand \
	bin/uniq \
	bin/unshar \
	bin/update \
	bin/uud \
	bin/uue \
	bin/vol \
	bin/wc \
	bin/whatsnew \
	bin/which \
	bin/who \
	bin/whoami \
	bin/width \
	bin/write \
	bin/xargs \
	bin/yes \

bin:
	mkdir bin

bin/add_route:	add_route.c
	$(CCLD) -o $@ add_route.c
	install -S 4kw $@

bin/ascii:	ascii.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/at:	at.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/atrun:	atrun.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/backup:	backup.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/badblocks:	badblocks.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/banner:	banner.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/basename:	basename.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/btoa:	btoa.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/cal:	cal.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/calendar:	calendar.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/cat:	cat.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/cdiff:	cdiff.c
	$(CCLD) -o $@ $?
	install -S 28kw $@

bin/cgrep:	cgrep.c
	$(CCLD) -o $@ $?
	install -S 5kw $@

bin/chmem:	chmem.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/chmod:	chmod.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/chown:	chown.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/ci:	ci.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/cksum:	cksum.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/clr:	clr.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/cmp:	cmp.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/co:	co.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/comm:	comm.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/compress:	compress.c
	$(CCLD) -o $@ $?
	install -S 450k $@

bin/cp:    cp.c
	$(CCLD) -o $@ $?
	install -S 16kw $@

bin/crc:	crc.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/cron:	cron.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/cut:	cut.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/date:	date.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/dd:	dd.c
	$(CCLD) -o $@ $?
	install -S 20kw $@

bin/decomp16:	decomp16.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/df:	df.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/dhrystone:	dhrystone.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/diff:	diff.c
	$(CCLD) -m -o $@ $?
	install -S 40kw $@

bin/dirname:	dirname.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/diskcheck:	diskcheck.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/diskusage:	diskusage.c
	$(CCLD) -o $@ $?
	install -S 25kw $@

bin/du:	du.c
	$(CCLD) -o $@ $?
	install -S 16kw $@

bin/dw:	dw.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/echo:	echo.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/ed:	ed.c
	$(CCLD) -o $@ $?
	install -S 32kw $@

bin/eject:	eject.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/expand:	expand.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/expr:	expr.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/factor:	factor.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/fgrep:	fgrep.c
	$(CCLD) -o $@ $?
	install -S 10kw $@

bin/file:	file.c
	$(CCLD) -o $@ $?
	install -S 25kw $@

bin/find:	find.c
	$(CCLD) -o $@ $?
	install -S 25kw $@

bin/finger:	finger.c
	$(CCLD) -m -o $@ finger.c
	install -S 8kw $@

bin/fold:	fold.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/fortune:	fortune.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/fsck:	fsck.c
	$(CCLD) -m -o $@ $?
	install -S 384k $@

bin/fsck1:	fsck1.c
	$(CCLD) -m -o $@ $?
	install -S 32kw $@

bin/gather:	gather.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/getty:	getty.c /usr/include/minix/config.h
	$(CCLD) -o $@ getty.c
	install -S 4kw $@

bin/gomoku:	gomoku.c
	$(CCLD) -o $@ $? -lcurses
	install -S 8kw $@

bin/grep:	grep.c
	$(CCLD) -o $@ $?
	install -S 32kw $@

bin/head:	head.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/host:	host.c
	$(CCLD) -m -wo -o $@ host.c
	install -S 4kw $@

bin/hostaddr:	hostaddr.c
	$(CCLD) -o $@ hostaddr.c
	install -S 4kw $@

bin/id:	id.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/ifconfig:	ifconfig.c
	$(CCLD) -o $@ ifconfig.c
	install -S 4kw $@

bin/ifdef:	ifdef.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/in.fingerd:	in.fingerd.c
	$(CCLD) -o $@ in.fingerd.c
	install -S 4kw $@

bin/in.rld:	in.rld.c
	$(CCLD) -m -o $@ in.rld.c
	install -S 4kw $@

bin/in.rshd:	in.rshd.c
	$(CCLD) -o $@ in.rshd.c
	install -S 4kw $@

bin/inodes:	inodes.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/install:	install.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/irdpd:	irdpd.c
	$(CCLD) -m -o $@ $?
	install -S 4kw $@

bin/isoread:	isoread.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/join:	join.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/kill:	kill.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/last:	last.c
	$(CCLD) -o $@ $?
	install -S 5kw $@

bin/leave:	leave.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/life:	life.c
	$(CCLD) -m -o $@ $? -lcurses
	install -S 15kw $@

bin/login:	login.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/look:	look.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/lp:	lp.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/lpd:	lpd.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/ls:	ls.c
	$(CCLD) -m -o $@ $?
	install -S 20kw $@

bin/mail:	mail.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/man:	man.c
	$(CCLD) -o $@ $?
	install -S 10kw $@

bin/men:	men.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/mesg:	mesg.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/mkdir:	mkdir.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/mkfifo:	mkfifo.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/mkfs:	mkfs.c
	$(CCLD) -m -o $@ $?
	install -S 20kw $@

bin/mknod:	mknod.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/mkproto:	mkproto.c
	$(CCLD) -o $@ $?
	install -S 20kw $@

bin/modem:	modem.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/mount:	mount.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/mref:	mref.c
	$(CCLD) -o $@ $?
	install -S 8kw $@

bin/mt:	mt.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/ncheck:	ncheck.c
	$(CCLD) -o $@ $?
	install -S 20kw $@

bin/nm:	nm.c
	$(CCLD) -o $@ $?
	install -S 32kw $@

bin/nonamed:	nonamed.c
	$(CCLD) -m -o $@ $?
	install -S 4kw $@

bin/od:	od.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/passwd:	passwd.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/paste:	paste.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/pathchk:	pathchk.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/ping:	ping.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/pr:	pr.c
	$(CCLD) -o $@ $?
	install -S 16kw $@

bin/pr_routes:	pr_routes.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/prep:	prep.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/pretty:	pretty.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/printenv:	printenv.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/printroot:	printroot.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/proto:	proto.c
	$(CCLD) -o $@ $?
	install -S 15kw $@

bin/pwd:	pwd.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/pwdauth:	pwdauth.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/rarpd:	rarpd.c
	$(CCLD) -m -o $@ rarpd.c
	install -S 4kw $@

bin/rcp:	rcp.c
	$(CCLD) -o $@ rcp.c
	install -S 8kw $@

bin/readall:	readall.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/readfs:	readfs.c
	$(CCLD) -o $@ $?
	install -S 25kw $@

bin/recover:	recover.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/remsync:	remsync.c
	$(CCLD) -o $@ $?
	install -S 256k $@

bin/rev:	rev.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/rlogin:	rlogin.c
	$(CCLD) -o $@ -m $?
	install -S 8kw $@

bin/rmdir:	rmdir.c
	$(CCLD) -o $@ $?
	install -S 15kw $@

bin/roff:	roff.c
	$(CCLD) -m -o $@ $?
	install -S 8kw $@

bin/rsh:	rsh.c
	$(CCLD) -o $@ rsh.c
	install -S 8kw $@

bin/sed:	sed.c
	$(CCLD) -o $@ $?
	install -S 8kw $@

bin/shar:	shar.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/size:	size.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/sleep:	sleep.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/sort:	sort.c
	$(CCLD) -o $@ $?
	install -S 30kw $@

bin/split:	split.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/strings:	strings.c
	$(CCLD) -o $@ $?
	install -S 8kw $@

bin/strip:	strip.c
	$(CCLD) -o $@ $?
	install -S 8kw $@

bin/stty:	stty.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/su:	su.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/sum:	sum.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/swapfs:	swapfs.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/sync:	sync.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/synctree:	synctree.c
	$(CCLD) -m -o $@ -wo $?
	install -S 32kw $@

bin/tail:	tail.c
	$(CCLD) -o $@ $?
	install -S 16kw $@

bin/tar:	tar.c
	$(CCLD) -o $@ $?
	install -S 30kw $@

bin/tcpd:	tcpd.c
	$(CCLD) -o $@ tcpd.c
	install -S 2kw $@

bin/tee:	tee.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/term:	term.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/termcap:	termcap.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/test:	test.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/tget:	tget.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/time:	time.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/touch:	touch.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/tr:	tr.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/traverse:	traverse.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/treecmp:	treecmp.c
	$(CCLD) -o $@ $?
	install -S 30kw $@

bin/tsort:	tsort.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/ttt:	ttt.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/tty:	tty.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/umount:	umount.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/uname:	uname.c /usr/include/minix/config.h
	$(CCLD) -o $@ uname.c
	install -S 4kw $@

bin/unexpand:	unexpand.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/uniq:	uniq.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/unshar:	unshar.c
	$(CCLD) -o $@ $?
	install -S 10kw $@

bin/update:	update.c
	$(CCLD) -o $@ $?
	install -S 1kw $@

bin/uud:	uud.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/uue:	uue.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/vol:	vol.c
	$(CCLD) -o $@ $?
	install -S 80k $@	# note: '-S' is upper limit to 'vol -m'

bin/wc:	wc.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/whatsnew:	whatsnew.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/which:	which.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/who:	who.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/whoami:	whoami.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/width:	width.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/write:	write.c
	$(CCLD) -o $@ $?

bin/xargs:	xargs.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

bin/yes:	yes.c
	$(CCLD) -o $@ $?
	install -S 4kw $@

install:	bin \
	/usr/bin/add_route \
	/usr/bin/ascii \
	/usr/bin/at \
	/usr/bin/atrun \
	/usr/bin/backup \
		/usr/bin/restore \
	/usr/bin/badblocks \
	/usr/bin/banner \
	/usr/bin/basename \
	/usr/bin/btoa \
	/usr/bin/cal \
	/usr/bin/calendar \
	/usr/bin/cat \
	/usr/bin/cdiff \
	/usr/bin/cgrep \
	/usr/bin/chmem \
	/usr/bin/chmod \
	/usr/bin/chown \
		/usr/bin/chgrp \
	/usr/bin/ci \
	/usr/bin/cksum \
	/usr/bin/clr \
	/usr/bin/cmp \
	/usr/bin/co \
	/usr/bin/comm \
	/usr/bin/compress \
		/usr/bin/uncompress \
		/usr/bin/zcat \
	/usr/bin/cp \
		/usr/bin/clone \
		/usr/bin/cpdir \
		/usr/bin/ln \
		/usr/bin/mv \
		/usr/bin/rm \
	/usr/bin/crc \
	/usr/bin/cron \
	/usr/bin/cut \
	/usr/bin/date \
	/usr/bin/dd \
	/usr/bin/decomp16 \
	/usr/bin/df \
	/usr/bin/dhrystone \
	/usr/bin/diff \
	/usr/bin/dirname \
	/usr/bin/diskcheck \
	/usr/bin/diskusage \
	/usr/bin/du \
	/usr/bin/dw \
	/usr/bin/echo \
	/usr/bin/ed \
	/usr/bin/eject \
	/usr/bin/expand \
	/usr/bin/expr \
	/usr/bin/factor \
	/usr/bin/fgrep \
	/usr/bin/file \
	/usr/bin/find \
	/usr/bin/finger \
	/usr/bin/fold \
	/usr/bin/fortune \
	/usr/bin/fsck \
	/usr/bin/fsck1 \
	/usr/bin/gather \
	/usr/bin/getty \
	/usr/bin/gomoku \
	/usr/bin/grep \
	/usr/bin/head \
	/usr/bin/host \
	/usr/bin/hostaddr \
	/usr/bin/id \
	/usr/bin/ifconfig \
	/usr/bin/ifdef \
	/usr/bin/in.fingerd \
	/usr/bin/in.rld \
	/usr/bin/in.rshd \
	/usr/bin/inodes \
	/usr/bin/install \
	/usr/bin/irdpd \
	/usr/bin/isoread \
		/usr/bin/isodir \
		/usr/bin/isoinfo \
	/usr/bin/join \
	/usr/bin/kill \
	/usr/bin/last \
	/usr/bin/leave \
	/usr/bin/life \
	/usr/bin/login \
	/usr/bin/look \
	/usr/bin/lp \
	/usr/bin/lpd \
	/usr/bin/ls \
	/usr/bin/mail \
	/usr/bin/man \
	/usr/bin/men \
	/usr/bin/mesg \
	/usr/bin/mkdir \
	/usr/bin/mkfifo \
	/usr/bin/mkfs \
	/usr/bin/mknod \
	/usr/bin/mkproto \
	/usr/bin/modem \
	/usr/bin/mount \
	/usr/bin/mref \
	/usr/bin/mt \
	/usr/bin/ncheck \
	/usr/bin/nm \
	/usr/bin/nonamed \
	/usr/bin/od \
	/usr/bin/passwd \
		/usr/bin/chfn \
		/usr/bin/chsh \
	/usr/bin/paste \
	/usr/bin/pathchk \
	/usr/bin/ping \
	/usr/bin/pr \
	/usr/bin/pr_routes \
	/usr/bin/prep \
	/usr/bin/pretty \
	/usr/bin/printenv \
	/usr/bin/printroot \
	/usr/bin/proto \
	/usr/bin/pwd \
	/usr/lib/pwdauth \
	/usr/bin/rarpd \
	/usr/bin/rcp \
	/usr/bin/readall \
	/usr/bin/readfs \
	/usr/bin/recover \
	/usr/bin/remsync \
	/usr/bin/rev \
	/usr/bin/rlogin \
	/usr/bin/rmdir \
	/usr/bin/roff \
	/usr/bin/rsh \
	/usr/bin/sed \
	/usr/bin/shar \
	/usr/bin/size \
	/usr/bin/sleep \
	/usr/bin/sort \
	/usr/bin/split \
	/usr/bin/strings \
	/usr/bin/strip \
	/usr/bin/stty \
	/usr/bin/su \
	/usr/bin/sum \
	/usr/bin/swapfs \
	/usr/bin/sync \
	/usr/bin/synctree \
	/usr/bin/tail \
	/usr/bin/tar \
	/usr/bin/tcpd \
	/usr/bin/tee \
	/usr/bin/term \
	/usr/bin/termcap \
	/usr/bin/test \
		/usr/bin/[ \
	/usr/bin/tget \
	/usr/bin/time \
	/usr/bin/touch \
	/usr/bin/tr \
	/usr/bin/traverse \
	/usr/bin/treecmp \
	/usr/bin/tsort \
	/usr/bin/ttt \
	/usr/bin/tty \
	/usr/bin/umount \
	/usr/bin/uname \
		/usr/bin/arch \
	/usr/bin/unexpand \
	/usr/bin/uniq \
	/usr/bin/unshar \
	/usr/bin/update \
	/usr/bin/uud \
		/usr/bin/uudecode \
	/usr/bin/uue \
		/usr/bin/uuencode \
	/usr/bin/vol \
	/usr/bin/wc \
	/usr/bin/whatsnew \
	/usr/bin/which \
	/usr/bin/who \
	/usr/bin/whoami \
	/usr/bin/width \
	/usr/bin/write \
	/usr/bin/xargs \
	/usr/bin/yes \
	/bin/cat \
	/bin/date \
	/bin/echo \
	/bin/expr \
	/bin/fsck \
	/bin/mount \
	/bin/printroot \
	/bin/pwd \
	/bin/sync \
	/bin/test \
		/bin/[ \
	/bin/umount \

/usr/bin/add_route:	bin/add_route
	install -cs -o bin $? $@

/usr/bin/ascii:	bin/ascii
	install -cs -o bin $? $@

/usr/bin/at:	bin/at
	install -cs -o root -m 4755 $? $@

/usr/bin/atrun:	bin/atrun
	install -cs -o bin $? $@

/usr/bin/backup:	bin/backup
	install -cs -o bin $? $@

/usr/bin/restore:	/usr/bin/backup
	install -l $? $@

/usr/bin/badblocks:	bin/badblocks
	install -cs -o bin $? $@

/usr/bin/banner:	bin/banner
	install -cs -o bin $? $@

/usr/bin/basename:	bin/basename
	install -cs -o bin $? $@

/usr/bin/btoa:	bin/btoa
	install -cs -o bin $? $@

/usr/bin/cal:	bin/cal
	install -cs -o bin $? $@

/usr/bin/calendar:	bin/calendar
	install -cs -o bin $? $@

/usr/bin/cat:	bin/cat
	install -cs -o bin $? $@

/usr/bin/cdiff:	bin/cdiff
	install -cs -o bin $? $@

/usr/bin/cgrep:	bin/cgrep
	install -cs -o bin $? $@

/usr/bin/chmem:	bin/chmem
	install -cs -o bin $? $@

/usr/bin/chmod:	bin/chmod
	install -cs -o bin $? $@

/usr/bin/chown:	bin/chown
	install -cs -o bin $? $@

/usr/bin/chgrp:	/usr/bin/chown
	install -l $? $@

/usr/bin/ci:	bin/ci
	install -cs -o bin $? $@

/usr/bin/cksum:	bin/cksum
	install -cs -o bin $? $@

/usr/bin/clr:	bin/clr
	install -cs -o bin $? $@

/usr/bin/cmp:	bin/cmp
	install -cs -o bin $? $@

/usr/bin/co:	bin/co
	install -cs -o bin $? $@

/usr/bin/comm:	bin/comm
	install -cs -o bin $? $@

/usr/bin/compress:	bin/compress
	install -cs -o bin $? $@

/usr/bin/uncompress /usr/bin/zcat:	/usr/bin/compress
	install -l $? $@

/usr/bin/cp:    bin/cp
	install -cs -o bin $? $@

/usr/bin/clone /usr/bin/cpdir \
/usr/bin/ln /usr/bin/mv /usr/bin/rm:	/usr/bin/cp
	install -l $? $@

/usr/bin/crc:	bin/crc
	install -cs -o bin $? $@

/usr/bin/cron:	bin/cron
	install -cs -o bin $? $@

/usr/bin/cut:	bin/cut
	install -cs -o bin $? $@

/usr/bin/date:	bin/date
	install -cs -o bin $? $@

/usr/bin/dd:	bin/dd
	install -cs -o bin $? $@

/usr/bin/decomp16:	bin/decomp16
	install -cs -o bin $? $@

/usr/bin/df:	bin/df
	install -cs -o root -m 4755 $? $@

/usr/bin/dhrystone:	bin/dhrystone
	install -cs -o bin $? $@

/usr/bin/diff:	bin/diff
	install -cs -o bin $? $@

/usr/bin/dirname:	bin/dirname
	install -cs -o bin $? $@

/usr/bin/diskcheck:	bin/diskcheck
	install -cs -o bin $? $@

/usr/bin/diskusage:	bin/diskusage
	install -cs -o bin $? $@

/usr/bin/du:	bin/du
	install -cs -o bin $? $@

/usr/bin/dw:	bin/dw
	install -cs -o bin $? $@

/usr/bin/echo:	bin/echo
	install -cs -o bin $? $@

/usr/bin/ed:	bin/ed
	install -cs -o bin $? $@

/usr/bin/eject:	bin/eject
	install -cs -o bin $? $@

/usr/bin/expand:	bin/expand
	install -cs -o bin $? $@

/usr/bin/expr:	bin/expr
	install -cs -o bin $? $@

/usr/bin/factor:	bin/factor
	install -cs -o bin $? $@

/usr/bin/fgrep:	bin/fgrep
	install -cs -o bin $? $@

/usr/bin/file:	bin/file
	install -cs -o bin $? $@

/usr/bin/find:	bin/find
	install -cs -o bin $? $@

/usr/bin/finger:	bin/finger
	install -cs -o bin $? $@

/usr/bin/fold:	bin/fold
	install -cs -o bin $? $@

/usr/bin/fortune:	bin/fortune
	install -cs -o bin $? $@

/usr/bin/fsck:	bin/fsck
	install -cs -o bin $? $@

/usr/bin/fsck1:	bin/fsck1
	install -cs -o bin $? $@

/usr/bin/gather:	bin/gather
	install -cs -o bin $? $@

/usr/bin/getty:	bin/getty
	install -cs -o bin $? $@

/usr/bin/gomoku:	bin/gomoku
	install -cs -o bin $? $@

/usr/bin/grep:	bin/grep
	install -cs -o bin $? $@

/usr/bin/head:	bin/head
	install -cs -o bin $? $@

/usr/bin/host:	bin/host
	install -cs -o bin $? $@

/usr/bin/hostaddr:	bin/hostaddr
	install -cs -o root -m 4755 $? $@

/usr/bin/id:	bin/id
	install -cs -o bin $? $@

/usr/bin/ifconfig:	bin/ifconfig
	install -cs -o bin $? $@

/usr/bin/ifdef:	bin/ifdef
	install -cs -o bin $? $@

/usr/bin/in.fingerd:	bin/in.fingerd
	install -cs -o bin $? $@

/usr/bin/in.rld:	bin/in.rld
	install -cs -o bin $? $@

/usr/bin/in.rshd:	bin/in.rshd
	install -cs -o bin $? $@

/usr/bin/inodes:	bin/inodes
	install -cs -o bin $? $@

/usr/bin/install:	bin/install
	install -cs -o root -m 4755 $? $@

/usr/bin/irdpd:	bin/irdpd
	install -cs -o bin $? $@

/usr/bin/isoread:	bin/isoread
	install -cs -o bin $? $@

/usr/bin/isodir /usr/bin/isoinfo:	/usr/bin/isoread
	install -l $? $@

/usr/bin/join:	bin/join
	install -cs -o bin $? $@

/usr/bin/kill:	bin/kill
	install -cs -o bin $? $@

/usr/bin/last:	bin/last
	install -cs -o bin $? $@

/usr/bin/leave:	bin/leave
	install -cs -o bin $? $@

/usr/bin/life:	bin/life
	install -cs -o bin $? $@

/usr/bin/login:	bin/login
	install -cs -o bin $? $@

/usr/bin/look:	bin/look
	install -cs -o bin $? $@

/usr/bin/lp:	bin/lp
	install -cs -o bin $? $@

/usr/bin/lpd:	bin/lpd
	install -cs -o daemon -m 4755 $? $@

/usr/bin/ls:	bin/ls
	install -cs -o bin $? $@

/usr/bin/mail:	bin/mail
	install -cs -o root -m 4755 $? $@

/usr/bin/man:	bin/man
	install -cs -o bin $? $@

/usr/bin/men:	bin/men
	install -cs -o bin $? $@

/usr/bin/mesg:	bin/mesg
	install -cs -o bin $? $@

/usr/bin/mkdir:	bin/mkdir
	install -cs -o bin $? $@

/usr/bin/mkfifo:	bin/mkfifo
	install -cs -o bin $? $@

/usr/bin/mkfs:	bin/mkfs
	install -cs -o bin $? $@

/usr/bin/mknod:	bin/mknod
	install -cs -o bin $? $@

/usr/bin/mkproto:	bin/mkproto
	install -cs -o bin $? $@

/usr/bin/modem:	bin/modem
	install -cs -o bin $? $@

/usr/bin/mount:	bin/mount
	install -cs -o root -m 4755 $? $@

/usr/bin/mref:	bin/mref
	install -cs -o bin $? $@

/usr/bin/mt:	bin/mt
	install -cs -o bin $? $@

/usr/bin/ncheck:	bin/ncheck
	install -cs -o bin $? $@

/usr/bin/nm:	bin/nm
	install -cs -o bin $? $@

/usr/bin/nonamed:	bin/nonamed
	install -cs -o bin $? $@

/usr/bin/od:	bin/od
	install -cs -o bin $? $@

/usr/bin/passwd:	bin/passwd
	install -cs -o root -m 4755 $? $@

/usr/bin/chfn /usr/bin/chsh:	/usr/bin/passwd
	install -l $? $@

/usr/bin/paste:	bin/paste
	install -cs -o bin $? $@

/usr/bin/pathchk:	bin/pathchk
	install -cs -o bin $? $@

/usr/bin/ping:	bin/ping
	install -cs -o root -m 4755 $? $@

/usr/bin/pr:	bin/pr
	install -cs -o bin $? $@

/usr/bin/pr_routes:	bin/pr_routes
	install -cs -o bin $? $@

/usr/bin/prep:	bin/prep
	install -cs -o bin $? $@

/usr/bin/pretty:	bin/pretty
	install -cs -o bin $? $@

/usr/bin/printenv:	bin/printenv
	install -cs -o bin $? $@

/usr/bin/printroot:	bin/printroot
	install -cs -o bin $? $@

/usr/bin/proto:	bin/proto
	install -cs -o bin $? $@

/usr/bin/pwd:	bin/pwd
	install -cs -o bin $? $@

/usr/lib/pwdauth:	bin/pwdauth
	install -cs -o root -m 4755 $? $@

/usr/bin/rarpd:	bin/rarpd
	install -cs -o bin $? $@

/usr/bin/rcp:	bin/rcp
	install -cs -o bin $? $@

/usr/bin/readall:	bin/readall
	install -cs -o bin $? $@

/usr/bin/readfs:	bin/readfs
	install -cs -o bin $? $@

/usr/bin/recover:	bin/recover
	install -cs -o root -m 4755 $? $@

/usr/bin/remsync:	bin/remsync
	install -cs -o bin $? $@

/usr/bin/rev:	bin/rev
	install -cs -o bin $? $@

/usr/bin/rlogin:	bin/rlogin
	install -cs -o bin $? $@

/usr/bin/rmdir:	bin/rmdir
	install -cs -o bin $? $@

/usr/bin/roff:	bin/roff
	install -cs -o bin $? $@

/usr/bin/rsh:	bin/rsh
	install -cs -o bin $? $@

/usr/bin/sed:	bin/sed
	install -cs -o bin $? $@

/usr/bin/shar:	bin/shar
	install -cs -o bin $? $@

/usr/bin/size:	bin/size
	install -cs -o bin $? $@

/usr/bin/sleep:	bin/sleep
	install -cs -o bin $? $@

/usr/bin/sort:	bin/sort
	install -cs -o bin $? $@

/usr/bin/split:	bin/split
	install -cs -o bin $? $@

/usr/bin/strings:	bin/strings
	install -cs -o bin $? $@

/usr/bin/strip:	bin/strip
	install -cs -o bin $? $@

/usr/bin/stty:	bin/stty
	install -cs -o bin $? $@

/usr/bin/su:	bin/su
	install -cs -o root -m 4755 $? $@

/usr/bin/sum:	bin/sum
	install -cs -o bin $? $@

/usr/bin/swapfs:	bin/swapfs
	install -cs -o bin $? $@

/usr/bin/sync:	bin/sync
	install -cs -o bin $? $@

/usr/bin/synctree:	bin/synctree
	install -cs -o bin $? $@

/usr/bin/tail:	bin/tail
	install -cs -o bin $? $@

/usr/bin/tar:	bin/tar
	install -cs -o bin $? $@

/usr/bin/tcpd:	bin/tcpd
	install -cs -o bin $? $@

/usr/bin/tee:	bin/tee
	install -cs -o bin $? $@

/usr/bin/term:	bin/term
	install -cs -o bin -g uucp -m 2755 $? $@

/usr/bin/termcap:	bin/termcap
	install -cs -o bin $? $@

/usr/bin/test:	bin/test
	install -cs -o bin $? $@

/usr/bin/[:	/usr/bin/test
	install -l $? $@

/usr/bin/tget:	bin/tget
	install -cs -o bin $? $@

/usr/bin/time:	bin/time
	install -cs -o bin $? $@

/usr/bin/touch:	bin/touch
	install -cs -o bin $? $@

/usr/bin/tr:	bin/tr
	install -cs -o bin $? $@

/usr/bin/traverse:	bin/traverse
	install -cs -o bin $? $@

/usr/bin/treecmp:	bin/treecmp
	install -cs -o bin $? $@

/usr/bin/tsort:	bin/tsort
	install -cs -o bin $? $@

/usr/bin/ttt:	bin/ttt
	install -cs -o bin $? $@

/usr/bin/tty:	bin/tty
	install -cs -o bin $? $@

/usr/bin/umount:	bin/umount
	install -cs -o root -m 4755 $? $@

/usr/bin/uname:	bin/uname
	install -cs -o bin $? $@

/usr/bin/arch:	/usr/bin/uname
	install -l $? $@

/usr/bin/unexpand:	bin/unexpand
	install -cs -o bin $? $@

/usr/bin/uniq:	bin/uniq
	install -cs -o bin $? $@

/usr/bin/unshar:	bin/unshar
	install -cs -o bin $? $@

/usr/bin/update:	bin/update
	install -cs -o bin $? $@

/usr/bin/uud:	bin/uud
	install -cs -o bin $? $@

/usr/bin/uudecode:	/usr/bin/uud
	install -l $? $@

/usr/bin/uue:	bin/uue
	install -cs -o bin $? $@

/usr/bin/uuencode:	/usr/bin/uue
	install -l $? $@

/usr/bin/vol:	bin/vol
	install -cs -o bin $? $@

/usr/bin/wc:	bin/wc
	install -cs -o bin $? $@

/usr/bin/whatsnew:	bin/whatsnew
	install -cs -o bin $? $@

/usr/bin/which:	bin/which
	install -cs -o bin $? $@

/usr/bin/who:	bin/who
	install -cs -o bin $? $@

/usr/bin/whoami:	bin/whoami
	install -cs -o bin $? $@

/usr/bin/width:	bin/width
	install -cs -o bin $? $@

/usr/bin/write:	bin/write
	install -cs -o bin -g tty -m 2755 $? $@

/usr/bin/xargs:	bin/xargs
	install -cs -o bin $? $@

/usr/bin/yes:	bin/yes
	install -cs -o bin $? $@

/bin/cat:	/usr/bin/cat
	install -lcs $? $@

/bin/date:	/usr/bin/date
	install -lcs $? $@

/bin/echo:	/usr/bin/echo
	install -lcs $? $@

/bin/expr:	/usr/bin/expr
	install -lcs $? $@

/bin/fsck:	/usr/bin/fsck
	install -lcs $? $@

/bin/mount:	/usr/bin/mount
	install -lcs $? $@

/bin/printroot:	/usr/bin/printroot
	install -lcs $? $@

/bin/pwd:	/usr/bin/pwd
	install -lcs $? $@

/bin/sync:	/usr/bin/sync
	install -lcs $? $@

/bin/test:	/usr/bin/test
	install -lcs $? $@

/bin/[:	/bin/test
	install -l $? $@

/bin/umount:	/usr/bin/umount
	install -lcs $? $@

clean:
	rm -rf a.out bin
