# SpacePoint Fusion Mouse Controller

A simple Python command line tool to connect the [SpacePoint Fusion](http://www.pnicorp.com/markets/gaming) by PNI as a mouse controller to Windows.

## Getting Started

To run this command line tool you need to [properly install Python](http://docs.python-guide.org/en/latest/starting/install/win/) and [install virtualenv](http://virtualenv.readthedocs.org/en/latest/index.html).

1. Create a virtual environment and activate it using Windows Powershell

 ```
PS C:\> cd \path\to\local\repository
PS local\repository> virtualenv venv
PS local\repository> venv\Scripts\activate
```

 If using Windows Powershell, the `activate` script is subject to the execution policies on the system. By default on Windows 7, the system’s excution policy is set to `Restricted`, meaning no scripts like the `activate` script are allowed to be executed. In order to use the script, you have to relax your system’s execution policy.

 ```PS C:\> Set-ExecutionPolicy RemoteSigned```

2. Install required packages

 ```(venv) PS local\repository> pip install -r requirements.txt```

3. Install the [Python for Windows extensions](http://sourceforge.net/projects/pywin32/files/)

 ```(venv) PS local\repository> easy_install path\to\exe```

4. Run the command line tool

 ```(venv) PS local\repository> python spacepoint.py```

5. Deactivate the virtual environment

 ```(venv) PS local\repository> deactivate```

## References

- [SpacePoint Scout User Manual](http://www.pnicorp.com/system/files/SpacePoint%20Scout%20User%20Manual%20r03.pdf)
- [User Manual SpacePoint Fusion](http://web.sensor-ic.com:8000/ZLXIAZAI/PNI/SpacePoint_Fusion_User_Manual_r1.pdf)
- [Easy Absolute Orientation: PNI SpacePoint Fusion in Python](http://eclecti.cc/hardware/easy-absolute-orientation-pni-spacepoint-fusion-in-python) 
- [pywinusb.hid](https://github.com/rene-aguirre/pywinusb)