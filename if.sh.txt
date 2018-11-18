#!/bin/bash

ping  192.168.10.250  -c 2

if  [ $? -eq 0 ]
then
ansible-playbook  sample.yml
else

echo  "Machine is not up and running"

fi 

