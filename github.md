## github PR��������

- ����Ĵ��붼��ʹ��git���а汾���������д��붼�й���
	github�ϣ����ÿλͬѧ���ȶ�Ҫע��һ��github�˺Ų����Hello��Ŀ��Ϥgit����

- ��Ϥ����git����Ͳ������Ķ�[gitbook](https://git-scm.com/book/zh/v2)

***
### PR��pull request)����

1. **����fork����**

	������Ҫfork����Ŀ��github��ҳ��
	![fork](resources/Image/fork.png)
	���fork��ť������forkһ����ͬ�������Լ���github��ҳ��

2. **clone����**

	fork����󣬼������Լ��Ŀ���������clone����
	clone��(https\ssh)���ַ�ʽ��ע������
	![clone](resources/Image/clone.png)

����`git clone [ͼƬ�еĵ�ַ]`

3. **������֧-�޸�-�ύ���Լ��Ĵ���**

	���ִ����ɾ����࣬��������ϰ�߲����ڴ���Ŀ��ʱ����ٳ�����
	
	��������������֧����һ����Ŀ������
	
	- master��֧��һ����Ȼ����Ŀռ䵫�ǲ�Ҫ�����Ͻ����޸ġ������ķ�֧��ֻ����pull,push,PR���롣
	- develop��֧��һ�������Լ������ķ�֧���������Ͻ��в��ԡ���֤���롣
	- topic��֧������������ʱ��֧����ɺϲ���develop��֧���в�����֤��
```bash
����git checkout -b develop master
����git checkout -b topic develop
����#edit file in topic branch
����#vim file.c
����#add && commit
����git commit -a -m "what u fixed"
����#merge to develop|master ready to PR
����git checkout develop
����git merge topic
����#push to your repo
����git push
```

4. **github��ҳ�ύPR**
	![NewPR](resources/Image/NewPR.png)
	
	![CreatePR](resources/Image/CreatePR.png)
	
5. **�ȴ���Ŀά�������Merge**