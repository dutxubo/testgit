ʹ��˵����

����ļ����޸�
��1������һ��ʹ�� git add readme.txt ����ض��ļ����ݴ������� git add . ��������ļ�
��2���������ʹ�� git commit -m "��һ���޸�"   �ύ�޸ģ������ݴ��������������ύ����ǰ��֧

git status ��ѯ�ļ��Ƿ񱻸���
git diff readme.txt ��ѯ�ض��ļ����޸�����


�汾����
��1���鿴�ύ����ʷ��¼ �� git log  ���� git log -pretty=oneline
��2���汾���ˣ�git reset --hard HEAD^  ������^�����ϼ����汾������  git reset --hard HEAD~1
��3�����˵����°汾�� git reset --hard �汾��
��4����ȡ�汾�ţ�git reflog 

�ύǰ�����޸�
��1��git checkout -- readme.txt �е� -- ����Ҫ�����û�� -- �Ļ�����ô�����ɴ�����֧��

ɾ���ļ�
��1��rm test.txt  ɾ����ʹ��commit�����ύ��ʹӰ汾���г���ɾ����
��2��git checkout  -- test.txt   ���ԴӰ汾���лָ��ļ�