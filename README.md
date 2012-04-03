Android Kernel Howto
--------------------

BEWARE: This kernel tree is made to be built in an android repo tree !

You MUST not use "make" in kernel/ directory but use the defined targets in the android repo root :

---

First you need to prepare the environment to tell we are building for the Defy

In gingerbread : 

  lunch cyanogen_jordan-eng

In ICS:

  lunch cm_jordan-userdebug

---

Then still in repo root folder, not kernel one, use one of these commands :

Available targets:

  make kernel_clean            # clean output

  make kernel                  # build the zImage

  make kernel_modules          # build the kernel modules

  make ext_kernel_modules      # build tiwlan modules (require system/wlan/ti git project)

  make kernel_modules_install  # copy the kernel modules to output folder system/lib/modules


---

'Tanguy Pruvot, March 2012'
