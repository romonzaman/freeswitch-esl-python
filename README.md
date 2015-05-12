# FreeSWITCH ESL Python

This is a python package to distribute the ESL.py module generated by FreeSWITCH. It's an auto-generated swig module and has a binary component. The idea is to make it easy to use the module on different boxes without having to download and installind FreeSWITCH. The required source and header files to generate _ESL.so are included.

## Installing

```shell
$ pip install git+https://github.com/victor-torres/freeswitch-esl-python.git
```

## Using

```python
from freeswitchESL import ESL
```

## Redundancy

```python
try:
    import ESL
except ImportError:
    from freeswitchESL import ESL
```

Redundancy could be helpful when you have FreeSWITCH running with your system in production environments, so you can just import ESL, but you also have a test environment (E.g. Codeship) without a FreeSWITCH installation.

## Resources

- Original repository by [gurteshwar](https://github.com/gurteshwar/freeswitch-esl-python)
- FreeSWITCH docs: [ESL](http://wiki.freeswitch.org/wiki/Esl)
- FreeSWICTH docs [Python ESL](http://wiki.freeswitch.org/wiki/Python_ESL)

## Notes

- Needs to be updated with fresh releases of FreeSWITCH
- But should run fine in production environments
