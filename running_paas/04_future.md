!SLIDE transition=fade
# The Future: Secure LXC

!SLIDE bold center
# LXC
![background](japanese_walls.png)

!SLIDE bold center
# SELinux
![background](norad.png)

!SLIDE bold
![background](cloud.png)

!SLIDE transition=fade
# The Present... 

!SLIDE
![background](wires.jpg)

!SLIDE transition=fade
# Baby Steps

!SLIDE commandline incremental transition=fade
# Step 1 - Unlearn this

	$ setenforce 0
	You know who you are...


!SLIDE condense commandline incremental transition=fade
# Step 2 - Learn the 'Z'

	$ ls -lZ
	drwxr-xr-x. mhicks mhicks unconfined_u:object_r:user_home_t:s0 about_me
	-rwxrwxr-x. mhicks mhicks unconfined_u:object_r:user_home_t:s0 config.ru
	drwxr-xr-x. mhicks mhicks unconfined_u:object_r:user_home_t:s0 experimental
	-rw-rw-r--. mhicks mhicks unconfined_u:object_r:user_home_t:s0 Gemfile
	-rw-rw-r--. mhicks mhicks unconfined_u:object_r:user_home_t:s0 Gemfile.lock
	drwxrwxr-x. mhicks mhicks unconfined_u:object_r:user_home_t:s0 public
	-rw-rw-r--. mhicks mhicks unconfined_u:object_r:user_home_t:s0 README.md
	drwxrwxr-x. mhicks mhicks unconfined_u:object_r:user_home_t:s0 running_paas
	-rw-rw-r--. mhicks mhicks unconfined_u:object_r:user_home_t:s0 script.js
	-rw-rw-r--. mhicks mhicks unconfined_u:object_r:user_home_t:s0 showoff.json
	-rw-rw-r--. mhicks mhicks unconfined_u:object_r:user_home_t:s0 styles.css
	drwxr-xr-x. mhicks mhicks unconfined_u:object_r:user_home_t:s0 title
	drwxrwxr-x. mhicks mhicks unconfined_u:object_r:user_home_t:s0 tmp

!SLIDE condense commandline incremental transition=fade
# Step 2 - Learn the 'Z' (cont.)

	$ ps -eZ
	LABEL                           PID       TTY       TIME        CMD
	unconfined_u:unconfined_r:unconfined_t:s0-s0:c0.c1023 9542 pts/2 00:00:00 bash
	unconfined_u:unconfined_r:unconfined_t:s0-s0:c0.c1023 9609 pts/2 00:00:00 ps -fZ

!SLIDE condense commandline incremental transition=fade
# Having trouble?

	$ grep -r "denied" /var/log/audit/audit.log
	See results?  If so, SELinux is blocking something...

!SLIDE transition=fade
![New Tool in the Belt](toolbelt.jpg)


!SLIDE bullets transition=fade
# Still Stuck?

* <http://fedoraproject.org/wiki/SELinux>

!SLIDE bullets transition=fade
# Next Step...

* [OpenShift Origin LiveCD](http://openshift.redhat.com/community/)
