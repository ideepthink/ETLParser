һ���ļ�˵����
	

����Դ����������Ҫ�޸ģ�
	��һ��com.teradata.sqlparser.parser.SqlParser�ࣺ
			���������һЩ�޸ģ����Ҳ�֪���������SqlParser���Ƿ�ͽ��е�һ�£��Ұ��ҵ��޸�����һ�£�����ͬ�¿ɽ�����Ӧ���޸�  
		1��bteqBridge������
			(1)������ʼ��sql_num_limit��ֵ�ĳ�ʼ������ȥ���ˣ����޸���Ϊ��������SQL���������е��������ݿⱣ����ʱ����
			(2)ɾ����finally���System.gc()����
			(3)��������ѭ��������Try�Ŀ���
		2��addRelation������
			���˷���ԭ������Insert���ķ�ʽ�޸�Ϊ����һ��VO�������ø�VO���󣬿�ѡ��ֱ�Ӳ�⡢����insert�ļ���������fastload�ļ���
			
	������tableRelationParser�ࣺ������޸ĺ�SqlParser��ͬ
	
���������ļ�˵�������������ļ���Ҫ�ŵ�����Ŀ¼�����ô����jar����
	1��log4j.properties ��־�����ļ�
	2��tap.properties ���ݿ����������ļ�
	3��parser.properties �������������ļ��������ļ����и�����˵��
		�������ļ�����Ҫ�޸����¼���������
		(1)targetpath������õ�Ŀ¼
		(2)logrinser.source����־���Ŀ¼
		(3)logrinser.perlcode�����ô���ȫ����־��������ѡ��Ĵ���ĳЩ�������־��
		(3)sqlparser.param���ɴ�ԭ���������ļ��п�������
		(4)sqlparser.writeDB���������Ƿ�ֱ��д�����ݿ�
	
�ġ���������
	java -Xms512m -Xmx1280m -jar etl-parser-1.0.0-jar-with-dependencies.jar
	
�塢���ɵ��ļ�˵��
	1��report.txt   ����ִ���������
	2��error_log.log   ��ϸ�Ĵ����¼
	3��performance_logs.log		��ϸ�����ܼ�¼
	4�������õ����Ŀ¼�л�����ϴ�����־�ļ������ɵ�insert����ļ�
	

	

				
	   