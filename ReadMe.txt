һ.�����汾��
�ٳ�ʼ��һ��Git�ֿ⣺git init
������ļ���Git�ֿ⣺1.git add<file> ; ?2.git commit
?��.ʱ�������
�ٲ鿴������״̬���ļ��Ƿ��޸Ĺ���git status
�ڲ鿴�޸ĵ����ݣ�git diff
1.�汾����
��HEAD:��ǰ�汾
��HEAD^:�ϸ��汾
�۶�λ�汾��git reset --hard commit_id
��git log������ǰ����git log���Բ鿴�ύ��ʷ���Ա�ȷ��Ҫ���˵��ĸ��汾
��git reflog��Ҫ�ط�δ������git reflog�鿴������ʷ���Ա�ȷ��Ҫ�ص�δ�����ĸ��汾��
2.���������ݴ���
�ٹ��������������ڵ������ܿ�����Ŀ¼�������ҵ�learngit�ļ��о���һ��������
�ڰ汾�⣺��������һ������Ŀ¼.git��������㹤����������Git�İ汾�⡣
���ݴ�����Git�İ汾������˺ܶණ������������Ҫ�ľ��ǳ�Ϊstage�����߽�index�����ݴ�����? ? ? ? ? ?
? ? ? ? ? ? ? ��һ������git add���ļ���ӽ�ȥ��ʵ���Ͼ��ǰ��ļ��޸���ӵ��ݴ�����
? ? ? ? ? ? ? �ڶ�������git commit�ύ���ģ�ʵ���Ͼ��ǰ��ݴ��������������ύ����ǰ��֧��
3.�����޸�
��ÿ���޸ģ������add���ݴ������Ͳ�����뵽commit��
4.�����޸�
��git checkout -- file���������������޸�
��git reset HEAD file�����ݴ������޸ĳ����������·Żع�����
5.ɾ���ļ�
��git rm���Ӱ汾����ɾ���ļ�
��.Զ�ֿ̲�
1.���Զ�̿�
�ٹ���һ��Զ�̿⣺git remote add origin git@server-name:path/repo-name.git
�ڹ������һ������master��֧���������ݣ�git push -u origin master
�۴˺�ÿ�α����ύ��ֻҪ�б�Ҫ���Ϳ���ʹ������git push origin master���������޸�
ps:����Զ�̿��ǿյģ����ǵ�һ������master��֧ʱ��������-u������Git������ѱ��ص�master��֧�������͵�Զ���µ�master��֧������ѱ��ص�master��֧��Զ�̵�master��֧�������������Ժ�����ͻ�����ȡʱ�Ϳ��Լ����
2.��Զ�̿��¡
��Ҫ��¡һ���ֿ⣬���ȱ���֪���ֿ�ĵ�ַ��Ȼ��ʹ��git clone�����¡
��Git֧�ֶ���Э�飬����https����ͨ��ssh֧�ֵ�ԭ��gitЭ���ٶ����
��.��֧����
1.������ϲ���֧
�ٲ鿴��֧��git branch
�ڴ�����֧��git branch<name>
���л���֧��git cheakout<name>
�ܴ���+�л���֧��git?cheakout -b?<name>
�ݺϲ�ĳ��֧����ǰ��֧��git merge<name>
��ɾ����֧��git branch - d <name>
2.�����ͻ
�ٲ鿴��֧�ϲ�ͼ��git log -- graph
? eg��git log --graph --pretty =oneline --abbrev -commit
3.��֧�������
�ٺϲ���֧ʱ��--no-ff��������ͨģʽ�ϲ����ϲ������ʷ�з�֧������fast forward
eg:git log --no-ff-m"merge with no--ff"dev
4.Bug��֧
��git stash���ѵ�ǰ�����ֳ�����������ȥ�޸�bug
��git stash pop���ָ������ֳ�ͬʱɾ��stash����
5.Feature��֧
�ٿ���һ����feature������½�һ����֧��
�����Ҫ����һ��û�б��ϲ����ķ�֧������ͨ��git branch -D <name>ǿ��ɾ��
6.����Э��
��git remote -v���鿴Զ�̿���Ϣ
��git push origin branch-name���ӱ������ͷ�֧
��git pull������ʧ��ʱ��ץȡԶ�̵����ύ
��git checkout -b branch-name origin/branch-name���ڱ��ش�����Զ�̷�֧��Ӧ�ķ�֧�����غ�Զ�̷�֧���������һ�£�
��git branch --set-upstream branch-name origin/branch-name���������ط�֧��Զ�̷�֧�Ĺ���
��.��ǩ����
1.������ǩ
��git tag <name>���½�һ����ǩ��Ĭ��ΪHEAD��Ҳ����ָ��commit id��
��git tag -a <tagname> -m "blablabla..."������ָ����ǩ��Ϣ
��git tag -s <tagname> -m "blablabla..."��������PGPǩ����Ϣ
��git tag���鿴���б�ǩ
2.������ǩ
��git push origin <tagname>������һ�����ر�ǩ
��git push origin --tags������ȫ��δ���͹��ı��ر�ǩ
��git tag -d <tagname>��ɾ��һ�����ر�ǩ
��git push origin :refs/tags/<tagname>��ɾ��һ��Զ�̱�ǩ
��.ʹ��GitHub
?
����GitHub�ϣ���������Fork��Դ�ֿ⣻
?
?
���Լ�ӵ��Fork��Ĳֿ�Ķ�дȨ�ޣ�
?
?
�ۿ�������pull request���ٷ��ֿ������״��롣
?
��.�Զ���Git
1.���������ļ�
�ٺ���ĳЩ�ļ�ʱ����Ҫ��д.gitignore��
2.���ñ���
������ֻ��Ҫ��һ���������Git���Ժ�st�ͱ�ʾstatus��git config --global alias.st status
?eg��
$ git config --global alias.co checkout
$ git config --global alias.ci commit
$ git config --global alias.br branch

$ git config --global alias.unstage 'reset HEAD'
$ git config --global alias.last 'log -1'

git config --global alias.lg "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"
3.�Git������
GitHub����һ������йܿ�Դ�����Զ�ֿ̲⡣���Ƕ���ĳЩ��Դ��������������ҵ��˾��˵���Ȳ��빫��Դ���룬���᲻�ø�GitHub�������ѣ��Ǿ�ֻ���Լ��һ̨Git��������Ϊ˽�вֿ�ʹ�á�
������ڵ���code.dianpingoa.com