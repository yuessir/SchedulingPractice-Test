# �Ƶ{�B�z���m��



# �ؼ�:

�Ҧ��Ƶ{���ɶ��w�Ƭ����A����b jobs �o table �� (schema �аѦҤU�軡��)�C�o�m�ߪ��D�n�ؼЬO�A�b jobs database �u�䴩�Q�ʬd�ߪ�����U�A
�г]�p worker �������ȡC

���Ȫ��ݨD (��������������):

1. �Ҧ� job �������b���w�ɶ��d�򤺳Q�Ұ� (�w���ɶ� + �i����������d��)
1. �C�� job ���u��Q����@��, ���঳�B�z��@�b���������p
1. �����䴩���������� (�h�� worker, ������t��, �ब�۳ƴ�, �䴩�ʺA scaling)

���_�B�z����~����� (�����u������):

1. ���������Ҧ��W�z���ȻݨD
1. Jobs �M��d�ߪ����ƶV�ֶV�n
1. Jobs ���հ��楢�� (�m����lock) �����ƶV�ֶV�n
1. Jobs ���𪺮ɶ��V�u�V�n (����: ��ڱҰʮɶ� - �w���Ұʮɶ�)
  * ���𥭧���, �V�p�V�n
  * ����зǮt, �V�p�V�n
1. �ӧO job ���A�d�ߪ����� (���w job id) �V�ֶV�n

�̲׵��� = Sum(���� x �v��):
1. ���榨��, �V�C�V�n:
```querylist x 100.0 + acquire_failure x 10.0 + queryjob x 1.0```
1. ����{��, �V�C�V�n:
```average + stdev```


# ���ҷǳ�