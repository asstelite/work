# Python 3.5.2

Create virtualenv

```
$ sudo apt-get install virtualenv
$ mkdir new_folder
$ cd new_folder/
$ virtualenv -p python3.5 venv
$ source venv/bin/activate
$ sudo apt-get install python3.5-dev
$ pip install -r requirements.txt
$ git clone https://github.com/asstelite/work.git
```

# task_1
1. In virtualenv:
```
  - Run by default arguments: $ python test_calculation.py
  - Run with arguments: $ python test_calculation.py -num1 any_number -num2 any_number
```

# task_2
1. In virtualenv:
```
  - Run with arguments:$ easypy job_file.py --num1 any_number --num2 any_number
```

# task_3
1.  my_testbed.yaml
```
- Write username, password, IP from task
```

2. Run job_ez.py with arguments in virtualenv:

```
arguments:
--vm_username - username of VM for connecting
--host_username - username of Host
--file_name - file name for creating and copying from VM to Host

$ easypy job_ez.py -testbed_file my_testbed.yaml --vm_username 'vm_name' --host_username 'hostname' --file_name 'file_name'
```

# task_4
1. In virtualenv:
```
  - Run with argument:$ easypy job_tests.py --letter 'write "a" or "b" or "c"'
```

# task_5
docker run -it -v $(pwd)/archive:/my-tests/archive my-tests easypy job_rabbit.py --word "any word"

