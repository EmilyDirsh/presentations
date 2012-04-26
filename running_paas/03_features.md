!SLIDE tech transition=fade
	@@@ Javascript

        {
          summary    : "What Developers Expect",

          language   : ['ruby' ,'python', 'perl'],

          scaling    : 'automagic',

          extensible : true,

          continuous_integration: true
        }

!SLIDE tech bullets incremental transition=fade

	@@@ Makefile
        Name: ops-expectations

        Summary: What Operations Expects

        Require: Multi-tenancy

        Require: Familiar installation

        %post
        echo "configuration=sane" > /etc/my.conf

!SLIDE transition=fade

# Multi-tenancy?

!SLIDE

![background](old_car.jpg)

!SLIDE

![background](fancy_car.jpg)

!SLIDE comic 

# Show me more!

!SLIDE bullets incremental transition=fade

# Containers

* SELinux
* Kernel Namespaces
* Linux Control Groups
* Bind Mounts
