# Vagrant and DNS Configuration Exercises

This repository contains exercises for setting up virtual machines and a Domain Name System (DNS) with Vagrant.

---

## Exercise 1

We are going to create the files `Vagrantfile` and `.gitignore` and configure `.gitignore` to ignore changes in the `.vagrant` and backup files as requested by the exercise.

Finally, I will also create the `README.md` file to document the exercises I am doing and the `LICENSE` file with a license of my choice.

---

## Exercise 2

We put the necessary instructions in the `Vagrantfile` to create the two virtual machines (venus and tierra) with their respective IP addresses.

Finally, we run `vagrant up` to create the Virtual Machines.

---

## Exercise 3

### Steps to Configure DNS

1. For sections 1, 2, and 3, we will configure the `named.conf.options` file. To do this, we will copy it outside the VM, modify it, and then copy it back to the machine.
2. For section 4, we will modify some files on the `tierra` machine to make it a master system.
3. For section 5, we will modify some files on the `venus` machine to make it a slave system.
4. For section 6, we have to configure a section of the `db.sistma.test` file which is “Negative Cache TTL”.
5. For section 7, we have to configure a section of the `named.conf.options` file so that unauthorized queries are forwarded to that IP.
6. For section 8, we will configure the `db.sistma.test` file to add the aliases as requested by the exercise.
7. For sections 9 and 10, we will configure the `db.sistma.test` file to add `marte` as the mail system as the exercise tells us to do.