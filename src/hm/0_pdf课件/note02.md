
<head>
    <meta charset="utf-8" />
    <title>
    </title>
    <link rel="stylesheet" type="text/css" href="030213212139_files/style.css" />
</head>
<body>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_04.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_04.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:7.6641em; left:4.0017em;"><span class="stl_07 stl_08 stl_09" style="font-weight:bold;">课程介绍 &nbsp;</span></div>
                <div class="stl_01" style="top:10.7384em; left:5.8775em;"><span class="stl_10 stl_08 stl_09">Nginx</span><span class="stl_11 stl_08 stl_09">日志分析系统 &nbsp;</span></div>
                <div class="stl_01" style="top:11.989em; left:5.8775em;"><span class="stl_10 stl_08 stl_09">Filebeat</span><span class="stl_11 stl_08 stl_09">入门学习 &nbsp;</span></div>
                <div class="stl_01" style="top:13.2395em; left:5.8775em;"><span class="stl_10 stl_08 stl_09">Metricbeat</span><span class="stl_11 stl_08 stl_09">入门学习 &nbsp;</span></div>
                <div class="stl_01" style="top:14.49em; left:5.8775em;"><span class="stl_10 stl_08 stl_09">Kibana</span><span class="stl_11 stl_08 stl_09">入门学习 &nbsp;</span></div>
                <div class="stl_01" style="top:15.7405em; left:5.8775em;"><span class="stl_10 stl_08 stl_09">Logstash</span><span class="stl_11 stl_08 stl_09">入门学习 &nbsp;</span></div>
                <div class="stl_01" style="top:16.9911em; left:5.8775em;"><span class="stl_11 stl_08 stl_09">综合练习 &nbsp;</span></div>
                <div class="stl_01" style="top:18.9813em; left:4.0017em;"><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">1</span><span class="stl_07 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">Nginx</span><span class="stl_07 stl_08 stl_09" style="font-weight:bold;">日志分析系统 &nbsp;</span></div>
                <div class="stl_01" style="top:22.0903em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">1</span></div>
                <div class="stl_01" style="top:22.0903em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.1</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、项目需求 &nbsp;</span></div>
                <div class="stl_01" style="top:24.5567em; left:4.0017em;"><span class="stl_10 stl_08 stl_09">Nginx</span><span class="stl_11 stl_08 stl_09">是一款非常优秀的</span><span class="stl_10 stl_08 stl_09">web</span><span class="stl_11 stl_08 stl_09">服务器，往往</span><span class="stl_10 stl_08 stl_09">nginx</span><span class="stl_11 stl_08 stl_09">服务会作为项目的访问入口，那么，</span><span class="stl_10 stl_08 stl_09">nginx</span><span class="stl_11 stl_08 stl_09">的性能保障就变得非常重 &nbsp;</span></div>
                <div class="stl_01" style="top:25.8073em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">要了，如果</span><span class="stl_10 stl_08 stl_09">nginx</span><span class="stl_11 stl_08 stl_09">的运行出现了问题就会对项目有较大的影响，所以，我们需要对</span><span class="stl_10 stl_08 stl_09">nginx</span><span class="stl_11 stl_08 stl_09">的运行有监控措施，实时掌握 &nbsp;</span></div>
                <div class="stl_01" style="top:27.0578em; left:4.0017em;"><span class="stl_10 stl_08 stl_09">nginx</span><span class="stl_11 stl_08 stl_09">的运行情况，那就需要收集</span><span class="stl_10 stl_08 stl_09">nginx</span><span class="stl_11 stl_08 stl_09">的运行指标和分析</span><span class="stl_10 stl_08 stl_09">nginx</span><span class="stl_11 stl_08 stl_09">的运行日志了。 &nbsp;</span></div>
                <div class="stl_01" style="top:29.1558em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">1</span></div>
                <div class="stl_01" style="top:29.1558em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.2</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、业务流程 &nbsp;</span></div>
                <div class="stl_01" style="top:55.1321em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">说明： &nbsp;</span></div>
                <div class="stl_01" style="top:57.0079em; left:5.8775em;"><span class="stl_11 stl_08 stl_09">通过</span><span class="stl_10 stl_08 stl_09">Beats</span><span class="stl_11 stl_08 stl_09">采集</span><span class="stl_10 stl_08 stl_09">Nginx</span><span class="stl_11 stl_08 stl_09">的指标数据和日志数据 &nbsp;</span></div>
                <div class="stl_01" style="top:58.2584em; left:5.8775em;"><span class="stl_10 stl_08 stl_15">Beats</span><span class="stl_11 stl_08 stl_15">采集到数据后发送到</span><span class="stl_10 stl_08 stl_15">Elasticsearch</span><span class="stl_11 stl_08 stl_15">中 &nbsp;</span></div>
                <div class="stl_01" style="top:59.5089em; left:5.8775em;"><span class="stl_10 stl_08 stl_09">Kibana</span><span class="stl_11 stl_08 stl_09">读取数据进行分析 &nbsp;</span></div>
                <div class="stl_01" style="top:60.7595em; left:5.8775em;"><span class="stl_11 stl_08 stl_09">用户通过</span><span class="stl_10 stl_08 stl_09">Kibana</span><span class="stl_11 stl_08 stl_09">进行查看分析报表 &nbsp;</span></div>
                <div class="stl_01" style="top:62.7497em; left:4.0017em;"><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">2</span><span class="stl_07 stl_08 stl_09" style="font-weight:bold;">、部署安装</span><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">Nginx &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_07.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_07.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:5.3668em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:6.4922em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:7.6177em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:8.7432em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:9.8687em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:10.9941em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:12.1196em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:13.2451em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:14.3705em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:5.3668em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">tar </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.001em;">-xvf </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">nginx-1.11.6.tar.gz &nbsp;</span></div>
                <div class="stl_01" style="top:6.4922em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">yum </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0004em;">-y </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">install pcre-devel zlib-devel &nbsp;</span></div>
                <div class="stl_01" style="top:7.6177em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">./configure &nbsp;</span></div>
                <div class="stl_01" style="top:8.7432em; left:6.8154em;"><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.001em;">make </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">install &nbsp;</span></div>
                <div class="stl_01" style="top:9.8687em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">启动 &nbsp;</span></div>
                <div class="stl_01" style="top:10.9941em; left:6.8154em;"><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.0005em;">cd </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;">/usr/local/nginx/sbin/ &nbsp;</span></div>
                <div class="stl_01" style="top:12.1196em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">./nginx &nbsp;</span></div>
                <div class="stl_01" style="top:14.3705em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">通过浏览器访问页面并且查看日志 &nbsp;</span></div>
                <div class="stl_01" style="top:15.496em; left:4.9337em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">10 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">访问地址：</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">http://192.168.40.133/ &nbsp;</span></div>
                <div class="stl_01" style="top:16.6215em; left:4.9337em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">11 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">tail</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0012em;"> -f</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;"> /usr/local/nginx/logs/access.log &nbsp;</span></div>
                <div class="stl_01" style="top:28.7979em; left:4.0017em;"><span class="stl_12 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">3</span><span class="stl_07 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">、</span><span class="stl_12 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">Beats </span><span class="stl_07 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">简介 &nbsp;</span></div>
                <div class="stl_01" style="top:62.3226em; left:4.0017em;"><span class="stl_11 stl_08 stl_24">官网：</span><a href="https://www.elastic.co/cn/products/beats" target="_blank"><span class="stl_25 stl_08 stl_24">https://www.elastic.co/cn/products/beats &nbsp;</span></a></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_10.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_10.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:25.3071em; left:4.0017em;"><span class="stl_10 stl_08 stl_09">Beats</span><span class="stl_11 stl_08 stl_09">系列产品： &nbsp;</span></div>
                <div class="stl_01" style="top:47.1181em; left:4.0017em;"><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">4</span><span class="stl_07 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">Filebeat &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_12.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_12.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:29.3434em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">4</span></div>
                <div class="stl_01" style="top:29.3434em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.1</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、架构 &nbsp;</span></div>
                <div class="stl_01" style="top:31.8098em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">用于监控、收集服务器日志文件</span><span class="stl_10 stl_08 stl_09">. &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_14.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_14.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:38.2846em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">4</span></div>
                <div class="stl_01" style="top:38.2846em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.2</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、部署与运行 &nbsp;</span></div>
                <div class="stl_01" style="top:40.7511em; left:4.0017em;"><span class="stl_11 stl_08 stl_26">下载（或使用资料中提供的安装包，版本为：</span><span class="stl_10 stl_08 stl_26">ﬁlebeat-6.5.4</span><span class="stl_11 stl_08 stl_26">）：</span><a href="https://www.elastic.co/downloads/beats" target="_blank"><span class="stl_25 stl_08 stl_26">https://www.elastic.co/downloads/beats &nbsp;</span></a></div>
                <div class="stl_01" style="top:43.3827em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:44.5082em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:45.6337em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:46.7591em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:47.8846em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:49.0101em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:50.1356em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:51.261em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:52.3865em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:53.512em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:43.3827em; left:6.8154em;"><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.0012em;">mkdir </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0012em;">/itcast/beats &nbsp;</span></div>
                <div class="stl_01" style="top:44.5082em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">tar </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.001em;">-xvf </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">filebeat-6.5.4-linux-x86_64.tar.gz &nbsp;</span></div>
                <div class="stl_01" style="top:45.6337em; left:6.8154em;"><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.0005em;">cd </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;">filebeat-6.5.4-linux-x86_64 &nbsp;</span></div>
                <div class="stl_01" style="top:47.8846em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0.3525em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.3525em;">创建如下配置文件 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.3525em;">itcast.yml &nbsp;</span></div>
                <div class="stl_01" style="top:49.0101em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">filebeat.inputs: &nbsp;</span></div>
                <div class="stl_01" style="top:50.1356em; left:6.8154em;"><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0001em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">type: stdin &nbsp;</span></div>
                <div class="stl_01" style="top:51.261em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0013em;">enabled: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0013em;">true &nbsp;</span></div>
                <div class="stl_01" style="top:52.3865em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">setup.template.settings: &nbsp;</span></div>
                <div class="stl_01" style="top:53.512em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0009em;">index.number_of_shards: </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0009em;">3 &nbsp;</span></div>
                <div class="stl_01" style="top:53.512em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:54.6375em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:55.7629em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:56.8884em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:58.0139em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:59.1394em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:60.2648em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:61.3903em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:62.5158em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:63.6413em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:54.6375em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">output.console: &nbsp;</span></div>
                <div class="stl_01" style="top:55.7629em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:56.8884em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:58.0139em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:55.7629em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0011em;">pretty: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0011em;">true &nbsp;</span></div>
                <div class="stl_01" style="top:56.8884em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0011em;">enable: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0011em;">true &nbsp;</span></div>
                <div class="stl_01" style="top:58.0139em; left:7.2562em;"><span class="stl_19 stl_08 stl_09">ꢀ</span></div>
                <div class="stl_01" style="top:59.1394em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">启动</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">filebeat &nbsp;</span></div>
                <div class="stl_01" style="top:60.2648em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">6 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">./filebeat</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0013em;"> -e</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0007em;"> -c</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;"> itcast.yml &nbsp;</span></div>
                <div class="stl_01" style="top:61.3903em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:62.5158em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">8 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">输入</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">hello</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">运行结果如下： &nbsp;</span></div>
                <div class="stl_01" style="top:63.6413em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">hello &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_15.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_15.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.804em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:5.9295em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:7.055em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:8.1805em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:9.3059em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:10.4314em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:11.5569em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:12.6823em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:13.8078em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:14.9333em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:16.0588em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:17.1842em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:18.3097em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:19.4352em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:20.5607em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:21.6861em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:22.8116em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:23.9371em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:25.0626em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:26.188em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:27.3135em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:28.439em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:29.5644em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:30.6899em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:31.8154em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:32.9409em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:4.804em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">{ &nbsp;</span></div>
                <div class="stl_01" style="top:5.9295em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:5.9295em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">ꢀ</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"@timestamp"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">: </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"2019-01-12T12:50:03.585Z"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:7.055em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"@metadata"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">: { </span><span class="stl_22 stl_08 stl_30" style="word-spacing:-0.0003em;">#</span><span class="stl_23 stl_08 stl_30" style="word-spacing:-0.0003em;">元数据信息 &nbsp;</span></div>
                <div class="stl_01" style="top:8.1805em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"beat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"filebeat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:9.3059em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0001em;">"type"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">: </span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0001em;">"doc"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:10.4314em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"version"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"6.5.4" &nbsp;</span></div>
                <div class="stl_01" style="top:11.5569em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:7.055em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:8.1805em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:9.3059em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:10.4314em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:11.5569em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:12.6823em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:12.6823em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0002em;">"source"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0002em;">""</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:13.8078em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:13.8078em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0002em;">"offset"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">: </span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0002em;">0</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:14.9333em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:14.9333em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"message"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"hello"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, ꢀ</span><span class="stl_22 stl_08 stl_30" style="word-spacing:0em;">#</span><span class="stl_23 stl_08 stl_30" style="word-spacing:0em;">输入的内容 &nbsp;</span></div>
                <div class="stl_01" style="top:16.0588em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">ꢀ</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"prospector"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">: { </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0004em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0004em;">标准输入勘探器 &nbsp;</span></div>
                <div class="stl_01" style="top:17.1842em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"type"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"stdin" &nbsp;</span></div>
                <div class="stl_01" style="top:18.3097em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:16.0588em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:17.1842em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:18.3097em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:19.4352em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:19.4352em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0003em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0003em;">"input"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0003em;">: { ꢀ</span><span class="stl_22 stl_08 stl_30" style="word-spacing:0.0003em;">#</span><span class="stl_23 stl_08 stl_30" style="word-spacing:0.0003em;">控制台标准输入 &nbsp;</span></div>
                <div class="stl_01" style="top:20.5607em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"type"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"stdin" &nbsp;</span></div>
                <div class="stl_01" style="top:21.6861em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:20.5607em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:21.6861em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:22.8116em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:22.8116em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">ꢀ</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"beat"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">: { </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0004em;">#beat</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0004em;">版本以及主机信息 &nbsp;</span></div>
                <div class="stl_01" style="top:23.9371em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"name"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"itcast01"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:25.0626em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"hostname"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"itcast01"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:26.188em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"version"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"6.5.4" &nbsp;</span></div>
                <div class="stl_01" style="top:27.3135em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:23.9371em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:25.0626em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:26.188em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:27.3135em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:28.439em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:28.439em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"host"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:29.5644em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:29.5644em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"name"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"itcast01" &nbsp;</span></div>
                <div class="stl_01" style="top:30.6899em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}</span></div>
                <div class="stl_01" style="top:30.6899em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:31.8154em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:32.9409em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:35.596em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">4</span></div>
                <div class="stl_01" style="top:35.596em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.3</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、读取文件 &nbsp;</span></div>
                <div class="stl_01" style="top:38.6308em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:39.7562em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:40.8817em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:42.0072em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:43.1326em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:44.2581em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:45.3836em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:46.5091em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:47.6346em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:38.6308em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0.3525em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.3525em;">配置读取文件项 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.3525em;">itcast-log.yml &nbsp;</span></div>
                <div class="stl_01" style="top:40.8817em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">filebeat.inputs: &nbsp;</span></div>
                <div class="stl_01" style="top:42.0072em; left:6.8154em;"><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0001em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">type: log &nbsp;</span></div>
                <div class="stl_01" style="top:43.1326em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0013em;">enabled: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0013em;">true &nbsp;</span></div>
                <div class="stl_01" style="top:44.2581em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">paths: &nbsp;</span></div>
                <div class="stl_01" style="top:45.3836em; left:8.5778em;"><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">/itcast/beats/logs/*.log &nbsp;</span></div>
                <div class="stl_01" style="top:46.5091em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">setup.template.settings: &nbsp;</span></div>
                <div class="stl_01" style="top:47.6346em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0009em;">index.number_of_shards: </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0009em;">3 &nbsp;</span></div>
                <div class="stl_01" style="top:48.76em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:49.8855em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:51.0109em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:52.1364em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:53.2619em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:54.3874em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:55.5129em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:56.6383em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:57.7638em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:58.8893em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:60.0147em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:61.1402em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:62.2657em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:63.3911em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:48.76em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">output.console: &nbsp;</span></div>
                <div class="stl_01" style="top:49.8855em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:51.0109em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:52.1364em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:49.8855em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0011em;">pretty: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0011em;">true &nbsp;</span></div>
                <div class="stl_01" style="top:51.0109em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0011em;">enable: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0011em;">true &nbsp;</span></div>
                <div class="stl_01" style="top:52.1364em; left:7.2562em;"><span class="stl_19 stl_08 stl_09">ꢀ</span></div>
                <div class="stl_01" style="top:53.2619em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">启动</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">filebeat &nbsp;</span></div>
                <div class="stl_01" style="top:54.3874em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">./filebeat</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0013em;"> -e</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0007em;"> -c</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;"> itcast-log.yml &nbsp;</span></div>
                <div class="stl_01" style="top:55.5129em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:56.6383em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">7 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#/haoke/beats/logs</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">下创建</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">a.log</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">文件，并输入如下内容 &nbsp;</span></div>
                <div class="stl_01" style="top:57.7638em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">8 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">hello &nbsp;</span></div>
                <div class="stl_01" style="top:58.8893em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">world &nbsp;</span></div>
                <div class="stl_01" style="top:60.0147em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:61.1402em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">观察</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">filebeat</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">输出 &nbsp;</span></div>
                <div class="stl_01" style="top:62.2657em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">{ &nbsp;</span></div>
                <div class="stl_01" style="top:63.3911em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:63.3911em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">ꢀ</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"@timestamp"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">: </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"2019-01-12T14:16:10.192Z"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_16.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_16.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.804em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:5.9295em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:7.055em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:8.1805em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:9.3059em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:10.4314em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:11.5569em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:12.6824em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:13.8078em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:14.9333em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:16.0588em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:17.1842em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:18.3097em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:19.4352em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:20.5607em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:21.6862em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:22.8116em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:23.9371em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:25.0625em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:26.188em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:27.3135em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:28.439em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:29.5644em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:30.6899em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:31.8154em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:32.9409em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:34.0663em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:35.1918em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:36.3173em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:37.4427em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:38.5682em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:39.6937em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:40.8192em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:41.9447em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:43.0701em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:44.1956em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:45.3211em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:46.4465em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:47.572em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:48.6975em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:49.823em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:50.9484em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:52.0739em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:53.1994em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:54.3249em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:55.4503em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:56.5758em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:57.7012em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:58.8267em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:4.804em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:4.804em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">ꢀ</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0003em;">"@metadata"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:5.9295em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"beat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"filebeat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:7.055em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0001em;">"type"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">: </span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0001em;">"doc"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:8.1805em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"version"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"6.5.4" &nbsp;</span></div>
                <div class="stl_01" style="top:9.3059em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:5.9295em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:7.055em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:8.1805em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:9.3059em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:10.4314em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:10.4314em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"host"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:11.5569em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:11.5569em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"name"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"itcast01" &nbsp;</span></div>
                <div class="stl_01" style="top:12.6824em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:12.6824em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:13.8078em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:13.8078em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;">"source"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;">"/haoke/beats/logs/a.log"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:14.9333em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0002em;">"offset"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">: </span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0002em;">0</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:14.9333em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:16.0588em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:16.0588em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"message"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"hello"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:17.1842em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"prospector"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:18.3097em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"type"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"log" &nbsp;</span></div>
                <div class="stl_01" style="top:19.4352em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:17.1842em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:18.3097em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:19.4352em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:20.5607em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:20.5607em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"input"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:21.6862em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:21.6862em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"type"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"log" &nbsp;</span></div>
                <div class="stl_01" style="top:22.8116em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:22.8116em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:23.9371em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:23.9371em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"beat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:25.0625em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:25.0625em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"version"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"6.5.4"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:26.188em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"name"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"itcast01"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:27.3135em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"hostname"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"itcast01" &nbsp;</span></div>
                <div class="stl_01" style="top:28.439em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}</span></div>
                <div class="stl_01" style="top:26.188em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:27.3135em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:28.439em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:29.5644em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">6 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:30.6899em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">7 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">{ &nbsp;</span></div>
                <div class="stl_01" style="top:31.8154em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:31.8154em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">ꢀ</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"@timestamp"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">: </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"2019-01-12T14:16:10.192Z"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:32.9409em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:32.9409em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">ꢀ</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0003em;">"@metadata"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:34.0663em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"beat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"filebeat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:35.1918em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0001em;">"type"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">: </span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0001em;">"doc"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:36.3173em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"version"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"6.5.4" &nbsp;</span></div>
                <div class="stl_01" style="top:37.4427em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:34.0663em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:35.1918em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:36.3173em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:37.4427em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:38.5682em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:38.5682em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"prospector"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:39.6937em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"type"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"log" &nbsp;</span></div>
                <div class="stl_01" style="top:40.8192em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:39.6937em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:40.8192em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:41.9447em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:41.9447em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"input"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:43.0701em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:43.0701em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"type"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"log" &nbsp;</span></div>
                <div class="stl_01" style="top:44.1956em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:44.1956em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:45.3211em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:45.3211em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"beat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:46.4465em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:46.4465em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"version"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"6.5.4"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:47.572em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"name"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"itcast01"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:48.6975em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"hostname"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"itcast01" &nbsp;</span></div>
                <div class="stl_01" style="top:49.823em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:47.572em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:48.6975em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:49.823em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:50.9484em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:50.9484em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"host"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:52.0739em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:52.0739em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"name"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"itcast01" &nbsp;</span></div>
                <div class="stl_01" style="top:53.1994em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:53.1994em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:54.3249em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:54.3249em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;">"source"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;">"/haoke/beats/logs/a.log"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:55.4503em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0002em;">"offset"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">: </span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0002em;">6</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:55.4503em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:56.5758em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:56.5758em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"message"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"world" &nbsp;</span></div>
                <div class="stl_01" style="top:57.7012em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:58.8267em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:61.4473em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">可以看出，已经检测到日志文件有更新，立刻就会读取到更新的内容，并且输出到控制台。 &nbsp;</span></div>
                <div class="stl_01" style="top:63.5453em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">4</span></div>
                <div class="stl_01" style="top:63.5453em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.4</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、自定义字段 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_17.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_17.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:5.3668em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:6.4923em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:7.6177em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:8.7432em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:9.8686em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:10.9941em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:12.1196em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:13.2451em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:14.3706em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:15.496em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:16.6215em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:5.3668em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0.3525em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.3525em;">配置读取文件项 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.3525em;">itcast-log.yml &nbsp;</span></div>
                <div class="stl_01" style="top:7.6177em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">filebeat.inputs: &nbsp;</span></div>
                <div class="stl_01" style="top:8.7432em; left:6.8154em;"><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0001em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">type: log &nbsp;</span></div>
                <div class="stl_01" style="top:9.8686em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0013em;">enabled: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0013em;">true &nbsp;</span></div>
                <div class="stl_01" style="top:10.9941em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">paths: &nbsp;</span></div>
                <div class="stl_01" style="top:12.1196em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_20 stl_08 stl_09" style="word-spacing:0em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">/itcast/beats/logs/*.log &nbsp;</span></div>
                <div class="stl_01" style="top:13.2451em; left:7.6969em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">tags: [</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0002em;">"web"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">] ꢀ </span><span class="stl_22 stl_08 stl_30" style="word-spacing:-0.0002em;">#</span><span class="stl_23 stl_08 stl_30" style="word-spacing:-0.0002em;">添加自定义</span><span class="stl_22 stl_08 stl_30" style="word-spacing:-0.0002em;">tag</span><span class="stl_23 stl_08 stl_30" style="word-spacing:-0.0002em;">，便于后续的处理 &nbsp;</span></div>
                <div class="stl_01" style="top:14.3706em; left:7.6969em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">fields: ꢀ</span><span class="stl_22 stl_08 stl_30" style="word-spacing:0.0002em;">#</span><span class="stl_23 stl_08 stl_30" style="word-spacing:0.0002em;">添加自定义字段 &nbsp;</span></div>
                <div class="stl_01" style="top:15.496em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:16.6215em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:17.747em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:18.8724em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:19.9979em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:21.1234em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:22.2489em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:23.3743em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:24.4998em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:25.6253em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:26.7508em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:27.8762em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:29.0017em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:30.1272em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:31.2526em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:32.3781em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:33.5036em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:34.6291em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:35.7546em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:36.88em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:38.0055em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:39.131em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:40.2564em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:41.3819em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:42.5074em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:43.6328em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:44.7583em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:45.8838em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:47.0093em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:48.1348em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:49.2602em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:50.3857em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:51.5111em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:52.6366em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:53.7621em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:54.8876em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:56.0131em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:57.1385em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:58.264em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:59.3895em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:60.5149em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:61.6404em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:62.7659em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:63.8914em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:15.496em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ from:</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> itcast-im &nbsp;</span></div>
                <div class="stl_01" style="top:16.6215em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0011em;">fields_under_root: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0011em;">true </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0011em;">#true</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0011em;">为添加到根节点，</span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0011em;">false</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0011em;">为添加到子节点中 &nbsp;</span></div>
                <div class="stl_01" style="top:17.747em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">setup.template.settings: &nbsp;</span></div>
                <div class="stl_01" style="top:18.8724em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0009em;">index.number_of_shards: </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0009em;">3 &nbsp;</span></div>
                <div class="stl_01" style="top:19.9979em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">output.console: &nbsp;</span></div>
                <div class="stl_01" style="top:18.8724em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:21.1234em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:22.2489em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:23.3743em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:21.1234em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0011em;">pretty: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0011em;">true &nbsp;</span></div>
                <div class="stl_01" style="top:22.2489em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0011em;">enable: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0011em;">true &nbsp;</span></div>
                <div class="stl_01" style="top:23.3743em; left:7.2562em;"><span class="stl_19 stl_08 stl_09">ꢀ</span></div>
                <div class="stl_01" style="top:24.4998em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">8 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">启动</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">filebeat &nbsp;</span></div>
                <div class="stl_01" style="top:25.6253em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">./filebeat</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0013em;"> -e</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0007em;"> -c</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;"> itcast-log.yml &nbsp;</span></div>
                <div class="stl_01" style="top:26.7508em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:27.8762em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#/haoke/beats/logs</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">下创建</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">a.log</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">文件，并输入如下内容 &nbsp;</span></div>
                <div class="stl_01" style="top:29.0017em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_28 stl_08 stl_09" style="word-spacing:0.7645em;">123 &nbsp;</span></div>
                <div class="stl_01" style="top:30.1272em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:31.2526em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">执行效果 &nbsp;</span></div>
                <div class="stl_01" style="top:32.3781em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">{ &nbsp;</span></div>
                <div class="stl_01" style="top:33.5036em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:33.5036em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">ꢀ</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"@timestamp"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">: </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"2019-01-12T14:37:19.845Z"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:34.6291em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:34.6291em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">ꢀ</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0003em;">"@metadata"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:35.7546em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"beat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"filebeat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:36.88em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0001em;">"type"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">: </span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0001em;">"doc"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:38.0055em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"version"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"6.5.4" &nbsp;</span></div>
                <div class="stl_01" style="top:39.131em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:35.7546em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:36.88em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:38.0055em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:39.131em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:40.2564em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:40.2564em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0002em;">"offset"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">: </span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0002em;">0</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:41.3819em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"tags"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: [ &nbsp;</span></div>
                <div class="stl_01" style="top:41.3819em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:42.5074em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:42.5074em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"haoke-im" &nbsp;</span></div>
                <div class="stl_01" style="top:43.6328em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">], &nbsp;</span></div>
                <div class="stl_01" style="top:43.6328em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:44.7583em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:44.7583em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"prospector"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:45.8838em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"type"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"log" &nbsp;</span></div>
                <div class="stl_01" style="top:47.0093em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:45.8838em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:47.0093em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:48.1348em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:48.1348em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"beat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:49.2602em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:49.2602em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"name"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"itcast01"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:50.3857em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"hostname"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"itcast01"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:51.5111em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"version"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"6.5.4" &nbsp;</span></div>
                <div class="stl_01" style="top:52.6366em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:50.3857em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:51.5111em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:52.6366em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:53.7621em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:53.7621em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"host"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:54.8876em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:54.8876em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"name"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"itcast01" &nbsp;</span></div>
                <div class="stl_01" style="top:56.0131em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:56.0131em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:57.1385em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:57.1385em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;">"source"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;">"/itcast/beats/logs/a.log"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:58.264em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:-0.0001em;">ꢀ</span><span class="stl_29 stl_08 stl_31" style="word-spacing:-0.0001em;">"message"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:-0.0001em;">: </span><span class="stl_29 stl_08 stl_31" style="word-spacing:-0.0001em;">"123"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:-0.0001em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:59.3895em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"input"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:58.264em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:59.3895em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:60.5149em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:60.5149em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"type"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"log" &nbsp;</span></div>
                <div class="stl_01" style="top:61.6404em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:61.6404em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:62.7659em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:62.7659em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">ꢀ</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"from"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">: </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"haoke-im" &nbsp;</span></div>
                <div class="stl_01" style="top:63.8914em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_19.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_19.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.9581em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">4</span></div>
                <div class="stl_01" style="top:4.9581em; left:4.6976em;"><span class="stl_13 stl_08 stl_32" style="font-weight:bold;">.5</span><span class="stl_14 stl_08 stl_32" style="font-weight:bold;">、输出到</span><span class="stl_13 stl_08 stl_32" style="font-weight:bold;">Elasticsearch &nbsp;</span></div>
                <div class="stl_01" style="top:7.9929em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:9.1184em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:10.2438em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:11.3693em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:12.4947em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:13.6202em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:14.7457em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:15.8712em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:16.9967em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:18.1221em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:7.9929em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"># itcast-log.yml &nbsp;</span></div>
                <div class="stl_01" style="top:9.1184em; left:6.8154em;"><span class="stl_27 stl_08 stl_30">filebeat.inputs</span><span class="stl_33 stl_08 stl_30">: &nbsp;</span></div>
                <div class="stl_01" style="top:10.2438em; left:6.8154em;"><span class="stl_33 stl_08 stl_31" style="word-spacing:-0.0002em;">- </span><span class="stl_27 stl_08 stl_31" style="word-spacing:-0.0002em;">type</span><span class="stl_33 stl_08 stl_31" style="word-spacing:-0.0002em;">: </span><span class="stl_19 stl_08 stl_31" style="word-spacing:-0.0002em;">log &nbsp;</span></div>
                <div class="stl_01" style="top:11.3693em; left:7.6969em;"><span class="stl_27 stl_08 stl_30" style="word-spacing:-0.0003em;">enabled</span><span class="stl_33 stl_08 stl_30" style="word-spacing:-0.0003em;">: </span><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0003em;">true &nbsp;</span></div>
                <div class="stl_01" style="top:12.4947em; left:7.6969em;"><span class="stl_27 stl_08 stl_30">paths</span><span class="stl_33 stl_08 stl_30">: &nbsp;</span></div>
                <div class="stl_01" style="top:13.6202em; left:7.2562em;"><span class="stl_33 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ -</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;"> /itcast/beats/logs/*.log &nbsp;</span></div>
                <div class="stl_01" style="top:14.7457em; left:7.6969em;"><span class="stl_27 stl_08 stl_30" style="word-spacing:0.0003em;">tags</span><span class="stl_33 stl_08 stl_30" style="word-spacing:0.0003em;">: [</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0003em;">"haoke-im"</span><span class="stl_33 stl_08 stl_30" style="word-spacing:0.0003em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:15.8712em; left:7.6969em;"><span class="stl_27 stl_08 stl_30">fields</span><span class="stl_33 stl_08 stl_30">: &nbsp;</span></div>
                <div class="stl_01" style="top:16.9967em; left:7.2562em;"><span class="stl_27 stl_08 stl_30" style="word-spacing:0.6026em;">ꢀ from</span><span class="stl_33 stl_08 stl_30" style="word-spacing:0.6026em;">:</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;"> haoke-im &nbsp;</span></div>
                <div class="stl_01" style="top:18.1221em; left:7.6969em;"><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0004em;">fields_under_root</span><span class="stl_33 stl_08 stl_09" style="word-spacing:-0.0004em;">: </span><span class="stl_34 stl_08 stl_09" style="word-spacing:-0.0004em;">false &nbsp;</span></div>
                <div class="stl_01" style="top:18.1221em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:19.2476em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:20.3731em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:21.4985em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:22.624em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:19.2476em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_27 stl_08 stl_09" style="word-spacing:0.7645em;">setup.template.settings</span><span class="stl_33 stl_08 stl_09" style="word-spacing:0.7645em;">: &nbsp;</span></div>
                <div class="stl_01" style="top:20.3731em; left:7.6969em;"><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0005em;">index.number_of_shards</span><span class="stl_33 stl_08 stl_09" style="word-spacing:-0.0005em;">: </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;">3 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0005em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0005em;">指定索引的分区数 &nbsp;</span></div>
                <div class="stl_01" style="top:21.4985em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7646em;">3 </span><span class="stl_27 stl_08 stl_09" style="word-spacing:0.7646em;">output.elasticsearch</span><span class="stl_33 stl_08 stl_09" style="word-spacing:0.7646em;">:</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7646em;"> #</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0004em;">指定</span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0004em;">ES</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0004em;">的配置 &nbsp;</span></div>
                <div class="stl_01" style="top:22.624em; left:7.6969em;"><span class="stl_27 stl_08 stl_09" style="word-spacing:0.0001em;">hosts</span><span class="stl_33 stl_08 stl_09" style="word-spacing:0.0001em;">: [</span><span class="stl_29 stl_08 stl_09" style="word-spacing:0.0001em;">"192.168.1.7:9200"</span><span class="stl_33 stl_08 stl_09" style="word-spacing:0.0001em;">,</span><span class="stl_29 stl_08 stl_09" style="word-spacing:0.0001em;">"192.168.1.7:9201"</span><span class="stl_33 stl_08 stl_09" style="word-spacing:0.0001em;">,</span><span class="stl_29 stl_08 stl_09" style="word-spacing:0.0001em;">"192.168.1.7:9202"</span><span class="stl_33 stl_08 stl_09" style="word-spacing:0.0001em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:20.3731em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:22.624em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:25.2446em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">在日志文件中输入新的内容进行测试： &nbsp;</span></div>
                <div class="stl_01" style="top:46.6285em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">查看数据： &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_21.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_21.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:43.3492em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">4</span></div>
                <div class="stl_01" style="top:43.3492em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.6</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">Filebeat</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">工作原理 &nbsp;</span></div>
                <div class="stl_01" style="top:45.8157em; left:4.0017em;"><span class="stl_10 stl_08 stl_35" style="word-spacing:0.006em;">Filebeat</span><span class="stl_11 stl_08 stl_35" style="word-spacing:0.006em;">由两个主要组件组成：</span><span class="stl_10 stl_08 stl_35" style="word-spacing:0.006em;">prospector </span><span class="stl_11 stl_08 stl_35" style="word-spacing:0.006em;">和 </span><span class="stl_10 stl_08 stl_35" style="word-spacing:0.006em;">harvester</span><span class="stl_11 stl_08 stl_35" style="word-spacing:0.006em;">。 &nbsp;</span></div>
                <div class="stl_01" style="top:47.6915em; left:5.8775em;"><span class="stl_10 stl_08 stl_09">harvester</span><span class="stl_11 stl_08 stl_09">： &nbsp;</span></div>
                <div class="stl_01" style="top:49.3797em; left:7.7533em;"><span class="stl_11 stl_08 stl_09">负责读取单个文件的内容。 &nbsp;</span></div>
                <div class="stl_01" style="top:50.6302em; left:7.7533em;"><span class="stl_11 stl_08 stl_09">如果文件在读取时被删除或重命名，</span><span class="stl_10 stl_08 stl_09">Filebeat</span><span class="stl_11 stl_08 stl_09">将继续读取文件。 &nbsp;</span></div>
                <div class="stl_01" style="top:51.8807em; left:5.8775em;"><span class="stl_10 stl_08 stl_36">prospector &nbsp;</span></div>
                <div class="stl_01" style="top:53.5064em; left:7.7533em;"><span class="stl_10 stl_08 stl_35" style="word-spacing:0.0011em;">prospector </span><span class="stl_11 stl_08 stl_35" style="word-spacing:0.0011em;">负责管理</span><span class="stl_10 stl_08 stl_35" style="word-spacing:0.0011em;">harvester</span><span class="stl_11 stl_08 stl_35" style="word-spacing:0.0011em;">并找到所有要读取的文件来源。 &nbsp;</span></div>
                <div class="stl_01" style="top:54.7569em; left:7.7533em;"><span class="stl_11 stl_08 stl_09">如果输入类型为日志，则查找器将查找路径匹配的所有文件，并为每个文件启动一个</span><span class="stl_10 stl_08 stl_09">harvester</span><span class="stl_11 stl_08 stl_09">。 &nbsp;</span></div>
                <div class="stl_01" style="top:56.0075em; left:7.7533em;"><span class="stl_10 stl_08 stl_35">Filebeat</span><span class="stl_11 stl_08 stl_35">目前支持两种</span><span class="stl_10 stl_08 stl_35">prospector</span><span class="stl_11 stl_08 stl_35">类型：</span><span class="stl_10 stl_08 stl_35">log</span><span class="stl_11 stl_08 stl_35">和</span><span class="stl_10 stl_08 stl_35">stdin</span><span class="stl_11 stl_08 stl_35">。 &nbsp;</span></div>
                <div class="stl_01" style="top:57.258em; left:5.8775em;"><span class="stl_10 stl_08 stl_09">Filebeat</span><span class="stl_11 stl_08 stl_09">如何保持文件的状态 &nbsp;</span></div>
                <div class="stl_01" style="top:58.9462em; left:7.7533em;"><span class="stl_10 stl_08 stl_09" style="word-spacing:0em;">Filebeat </span><span class="stl_11 stl_08 stl_09" style="word-spacing:0em;">保存每个文件的状态并经常将状态刷新到磁盘上的注册文件中。 &nbsp;</span></div>
                <div class="stl_01" style="top:60.1967em; left:7.7533em;"><span class="stl_11 stl_08 stl_09">该状态用于记住</span><span class="stl_10 stl_08 stl_09">harvester</span><span class="stl_11 stl_08 stl_09">正在读取的最后偏移量，并确保发送所有日志行。 &nbsp;</span></div>
                <div class="stl_01" style="top:61.4472em; left:7.7533em;"><span class="stl_11 stl_08 stl_37">如果输出（例如</span><span class="stl_10 stl_08 stl_37">Elasticsearch</span><span class="stl_11 stl_08 stl_37">或</span><span class="stl_10 stl_08 stl_37">Logstash</span><span class="stl_11 stl_08 stl_37">）无法访问，</span><span class="stl_10 stl_08 stl_37">Filebeat</span><span class="stl_11 stl_08 stl_37">会跟踪最后发送的行，并在输出再次可用 &nbsp;</span></div>
                <div class="stl_01" style="top:62.6978em; left:7.7533em;"><span class="stl_11 stl_08 stl_09">时继续读取文件。 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_22.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_22.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.9235em; left:7.7533em;"><span class="stl_11 stl_08 stl_37">在</span><span class="stl_10 stl_08 stl_37">Filebeat</span><span class="stl_11 stl_08 stl_37">运行时，每个</span><span class="stl_10 stl_08 stl_37">prospector</span><span class="stl_11 stl_08 stl_37">内存中也会保存的文件状态信息，当重新启动</span><span class="stl_10 stl_08 stl_37">Filebeat</span><span class="stl_11 stl_08 stl_37">时，将使用注册 &nbsp;</span></div>
                <div class="stl_01" style="top:6.174em; left:7.7533em;"><span class="stl_11 stl_08 stl_09">文件的数据来重建文件状态，</span><span class="stl_10 stl_08 stl_09">Filebeat</span><span class="stl_11 stl_08 stl_09">将每个</span><span class="stl_10 stl_08 stl_09">harvester</span><span class="stl_11 stl_08 stl_09">在从保存的最后偏移量继续读取。 &nbsp;</span></div>
                <div class="stl_01" style="top:7.4246em; left:7.7533em;"><span class="stl_11 stl_08 stl_38">文件状态记录在</span><span class="stl_10 stl_08 stl_38">data/registry</span><span class="stl_11 stl_08 stl_38">文件中。 &nbsp;</span></div>
                <div class="stl_01" style="top:9.3003em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">启动命令： &nbsp;</span></div>
                <div class="stl_01" style="top:11.932em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:13.0575em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:14.183em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:15.3084em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:16.4339em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:17.5594em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:18.6849em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:19.8103em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:20.9358em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:22.0613em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:23.1868em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:24.3122em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:25.4377em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:26.5631em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:27.6886em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:28.8141em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:29.9396em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:31.0651em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:32.1905em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:33.316em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:34.4415em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:35.5669em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:36.6924em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:37.8179em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:38.9434em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:40.0688em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:41.1943em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:42.3198em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:43.4453em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:44.5707em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:45.6962em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:46.8217em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:47.9471em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:49.0726em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:50.1981em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:51.3236em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:52.4491em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:53.5745em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:54.7em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:11.932em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0008em;">./filebeat </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0008em;">-e -c </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0008em;">itcast.yml &nbsp;</span></div>
                <div class="stl_01" style="top:13.0575em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0007em;">./filebeat </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0007em;">-e -c </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0007em;">itcast.yml </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0007em;">-d </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0007em;">"publish" &nbsp;</span></div>
                <div class="stl_01" style="top:15.3084em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">参数说明 &nbsp;</span></div>
                <div class="stl_01" style="top:16.4339em; left:7.256em;"><span class="stl_20 stl_08 stl_09" style="word-spacing:0em;">-e</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">: </span><span class="stl_39 stl_08 stl_09" style="word-spacing:0em;">输出到标准输出，默认输出到</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">syslog</span><span class="stl_39 stl_08 stl_09" style="word-spacing:0em;">和</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">logs</span><span class="stl_39 stl_08 stl_09" style="word-spacing:0em;">下 &nbsp;</span></div>
                <div class="stl_01" style="top:17.5594em; left:7.256em;"><span class="stl_20 stl_08 stl_30" style="word-spacing:0.0001em;">-c</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">: </span><span class="stl_39 stl_08 stl_30" style="word-spacing:0.0001em;">指定配置文件 &nbsp;</span></div>
                <div class="stl_01" style="top:18.6849em; left:7.256em;"><span class="stl_20 stl_08 stl_09" style="word-spacing:0.0001em;">-d</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">: </span><span class="stl_39 stl_08 stl_09" style="word-spacing:0.0001em;">输出</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">debug</span><span class="stl_39 stl_08 stl_09" style="word-spacing:0.0001em;">信息 &nbsp;</span></div>
                <div class="stl_01" style="top:20.9358em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0.3525em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.3525em;">测试： </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.3525em;">./filebeat</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> -e</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> -c itcast-log.yml</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> -d</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> "publish" &nbsp;</span></div>
                <div class="stl_01" style="top:22.0613em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:23.1868em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:24.3122em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:25.4377em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:26.5631em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:27.6886em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:28.8141em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:29.9396em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:31.0651em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:32.1905em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:33.316em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:34.4415em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:35.5669em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:36.6924em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:37.8179em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:38.9434em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:40.0688em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:41.1943em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:42.3198em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:43.4453em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:44.5707em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:45.6962em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:46.8217em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:47.9471em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:49.0726em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:50.1981em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:51.3236em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:52.4491em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:53.5745em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:54.7em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:55.8255em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:56.9509em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:22.0613em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">DEBUG ꢀ [publish] ꢀ ꢀ ꢀ pipeline/processor.go:308 ꢀ ꢀ ꢀ Publish event: { &nbsp;</span></div>
                <div class="stl_01" style="top:23.1868em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">ꢀ</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"@timestamp"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">: </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"2019-01-12T15:03:50.820Z"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:24.3122em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">ꢀ</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0003em;">"@metadata"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:25.4377em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"beat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"filebeat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:26.5631em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0001em;">"type"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">: </span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0001em;">"doc"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:27.6886em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"version"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"6.5.4" &nbsp;</span></div>
                <div class="stl_01" style="top:28.8141em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:29.9396em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0002em;">"offset"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">: </span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0002em;">0</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:31.0651em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"tags"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: [ &nbsp;</span></div>
                <div class="stl_01" style="top:32.1905em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"haoke-im" &nbsp;</span></div>
                <div class="stl_01" style="top:33.316em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">], &nbsp;</span></div>
                <div class="stl_01" style="top:34.4415em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"input"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:35.5669em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"type"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"log" &nbsp;</span></div>
                <div class="stl_01" style="top:36.6924em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:37.8179em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"prospector"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:38.9434em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"type"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"log" &nbsp;</span></div>
                <div class="stl_01" style="top:40.0688em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:41.1943em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"beat"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:42.3198em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"name"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"itcast01"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:43.4453em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"hostname"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"itcast01"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:44.5707em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"version"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"6.5.4" &nbsp;</span></div>
                <div class="stl_01" style="top:45.6962em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:46.8217em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;">"source"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;">"/haoke/beats/logs/a.log"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:47.9471em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"fields"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:49.0726em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"from"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"haoke-im" &nbsp;</span></div>
                <div class="stl_01" style="top:50.1981em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:51.3236em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"host"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">: { &nbsp;</span></div>
                <div class="stl_01" style="top:52.4491em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"name"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"itcast01" &nbsp;</span></div>
                <div class="stl_01" style="top:53.5745em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">}, &nbsp;</span></div>
                <div class="stl_01" style="top:54.7em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"message"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">: </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"456" &nbsp;</span></div>
                <div class="stl_01" style="top:55.8255em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:56.9509em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:59.6061em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">4</span></div>
                <div class="stl_01" style="top:59.6061em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.7</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、读取</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">Nginx</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">日志文件 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_25.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_25.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:5.3668em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:6.4922em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:7.6177em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:8.7432em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:9.8686em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:10.9941em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:12.1196em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:13.2451em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:14.3706em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:5.3668em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"># itcast-nginx.yml &nbsp;</span></div>
                <div class="stl_01" style="top:6.4922em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">filebeat.inputs: &nbsp;</span></div>
                <div class="stl_01" style="top:7.6177em; left:6.8154em;"><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0001em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">type: log &nbsp;</span></div>
                <div class="stl_01" style="top:8.7432em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0013em;">enabled: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0013em;">true &nbsp;</span></div>
                <div class="stl_01" style="top:9.8686em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">paths: &nbsp;</span></div>
                <div class="stl_01" style="top:10.9941em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_20 stl_08 stl_09" style="word-spacing:0em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">/usr/local/nginx/logs/*.log &nbsp;</span></div>
                <div class="stl_01" style="top:12.1196em; left:7.6969em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">tags: [</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"nginx"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:13.2451em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">setup.template.settings: &nbsp;</span></div>
                <div class="stl_01" style="top:14.3706em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0007em;">index.number_of_shards: </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0007em;">3 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0007em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0007em;">指定索引的分区数 &nbsp;</span></div>
                <div class="stl_01" style="top:15.496em; left:4.9337em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">10 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">output.elasticsearch:</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;"> #</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0013em;">指定</span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0013em;">ES</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0013em;">的配置 &nbsp;</span></div>
                <div class="stl_01" style="top:16.6215em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">11 &nbsp;</span></div>
                <div class="stl_01" style="top:16.6215em; left:7.6969em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">hosts: [</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"192.168.40.133:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">,</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"192.168.40.134:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">,</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"192.168.40.135:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:19.6853em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:20.8108em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:19.6853em; left:6.3152em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">启动 &nbsp;</span></div>
                <div class="stl_01" style="top:20.8108em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0008em;">./filebeat </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0008em;">-e -c </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0008em;">itcast-nginx.yml &nbsp;</span></div>
                <div class="stl_01" style="top:41.0636em; left:4.0017em;"><span class="stl_11 stl_08 stl_35">启动后，可以在</span><span class="stl_10 stl_08 stl_35">Elasticsearch</span><span class="stl_11 stl_08 stl_35">中看到索引以及查看数据： &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_27.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_27.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:42.1892em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">可以看到，在</span><span class="stl_10 stl_08 stl_09">message</span><span class="stl_11 stl_08 stl_09">中已经获取到了</span><span class="stl_10 stl_08 stl_09">nginx</span><span class="stl_11 stl_08 stl_09">的日志，但是，内容并没有经过处理，只是读取到原数据，那么对于我 &nbsp;</span></div>
                <div class="stl_01" style="top:43.4397em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">们后期的操作是不利的，有办法解决吗？ &nbsp;</span></div>
                <div class="stl_01" style="top:45.5377em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">4</span></div>
                <div class="stl_01" style="top:45.5377em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.7</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">Module &nbsp;</span></div>
                <div class="stl_01" style="top:48.0042em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">前面要想实现日志数据的读取以及处理都是自己手动配置的，其实，在</span><span class="stl_10 stl_08 stl_09">Filebeat</span><span class="stl_11 stl_08 stl_09">中，有大量的</span><span class="stl_10 stl_08 stl_09">Module</span><span class="stl_11 stl_08 stl_09">，可以简化我 &nbsp;</span></div>
                <div class="stl_01" style="top:49.2546em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">们的配置，直接就可以使用，如下： &nbsp;</span></div>
                <div class="stl_01" style="top:51.8863em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:53.0118em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:54.1373em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:55.2628em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:56.3883em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:57.5137em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:58.6392em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:59.7646em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:60.8901em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:51.8863em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">./filebeat modules list &nbsp;</span></div>
                <div class="stl_01" style="top:54.1373em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">Enabled: &nbsp;</span></div>
                <div class="stl_01" style="top:56.3883em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">Disabled: &nbsp;</span></div>
                <div class="stl_01" style="top:57.5137em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">apache2 &nbsp;</span></div>
                <div class="stl_01" style="top:58.6392em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">auditd &nbsp;</span></div>
                <div class="stl_01" style="top:59.7646em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">elasticsearch &nbsp;</span></div>
                <div class="stl_01" style="top:60.8901em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">haproxy &nbsp;</span></div>
                <div class="stl_01" style="top:62.0156em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:63.141em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:64.2665em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:62.0156em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">icinga &nbsp;</span></div>
                <div class="stl_01" style="top:63.141em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">iis &nbsp;</span></div>
                <div class="stl_01" style="top:64.2665em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">kafka &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_28.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_28.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.804em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:5.9295em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:7.0549em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:8.1804em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:9.3059em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:10.4314em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:11.5569em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:12.6823em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:13.8078em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:14.9333em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:16.0588em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:17.1842em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:4.804em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">kibana &nbsp;</span></div>
                <div class="stl_01" style="top:5.9295em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">logstash &nbsp;</span></div>
                <div class="stl_01" style="top:7.0549em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">mongodb &nbsp;</span></div>
                <div class="stl_01" style="top:8.1804em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">6 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">mysql &nbsp;</span></div>
                <div class="stl_01" style="top:9.3059em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">7 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">nginx &nbsp;</span></div>
                <div class="stl_01" style="top:10.4314em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">8 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">osquery &nbsp;</span></div>
                <div class="stl_01" style="top:11.5569em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">postgresql &nbsp;</span></div>
                <div class="stl_01" style="top:12.6823em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">redis &nbsp;</span></div>
                <div class="stl_01" style="top:13.8078em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">suricata &nbsp;</span></div>
                <div class="stl_01" style="top:14.9333em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">system &nbsp;</span></div>
                <div class="stl_01" style="top:16.0588em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">traefik &nbsp;</span></div>
                <div class="stl_01" style="top:17.1842em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:19.8048em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">可以看到，内置了很多的</span><span class="stl_10 stl_08 stl_09">module</span><span class="stl_11 stl_08 stl_09">，但是都没有启用，如果需要启用需要进行</span><span class="stl_10 stl_08 stl_09">enable</span><span class="stl_11 stl_08 stl_09">操作： &nbsp;</span></div>
                <div class="stl_01" style="top:22.4364em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:23.5619em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:24.6873em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:25.8128em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:26.9383em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:28.0638em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:29.1893em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:30.3147em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:31.4402em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:22.4364em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">./filebeat modules enable nginx </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0003em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0003em;">启动 &nbsp;</span></div>
                <div class="stl_01" style="top:23.5619em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">./filebeat modules disable nginx </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0003em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0003em;">禁用 &nbsp;</span></div>
                <div class="stl_01" style="top:25.8128em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">Enabled: &nbsp;</span></div>
                <div class="stl_01" style="top:26.9383em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">nginx &nbsp;</span></div>
                <div class="stl_01" style="top:29.1893em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">Disabled: &nbsp;</span></div>
                <div class="stl_01" style="top:30.3147em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">apache2 &nbsp;</span></div>
                <div class="stl_01" style="top:31.4402em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">auditd &nbsp;</span></div>
                <div class="stl_01" style="top:32.5657em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:33.6912em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:34.8166em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:35.9421em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:37.0675em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:38.193em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:39.3185em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:40.444em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:41.5695em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:42.6949em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:43.8204em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:44.9459em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:46.0714em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:47.1969em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:48.3223em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:32.5657em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">elasticsearch &nbsp;</span></div>
                <div class="stl_01" style="top:33.6912em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">haproxy &nbsp;</span></div>
                <div class="stl_01" style="top:34.8166em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">icinga &nbsp;</span></div>
                <div class="stl_01" style="top:35.9421em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">iis &nbsp;</span></div>
                <div class="stl_01" style="top:37.0675em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">kafka &nbsp;</span></div>
                <div class="stl_01" style="top:38.193em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">kibana &nbsp;</span></div>
                <div class="stl_01" style="top:39.3185em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">6 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">logstash &nbsp;</span></div>
                <div class="stl_01" style="top:40.444em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">7 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">mongodb &nbsp;</span></div>
                <div class="stl_01" style="top:41.5695em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">8 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">mysql &nbsp;</span></div>
                <div class="stl_01" style="top:42.6949em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">redis &nbsp;</span></div>
                <div class="stl_01" style="top:43.8204em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:43.8204em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">osquery &nbsp;</span></div>
                <div class="stl_01" style="top:44.9459em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">postgresql &nbsp;</span></div>
                <div class="stl_01" style="top:46.0714em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">suricata &nbsp;</span></div>
                <div class="stl_01" style="top:47.1969em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">system &nbsp;</span></div>
                <div class="stl_01" style="top:48.3223em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">traefik &nbsp;</span></div>
                <div class="stl_01" style="top:50.9428em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">可以发现，</span><span class="stl_10 stl_08 stl_09">nginx</span><span class="stl_11 stl_08 stl_09">的</span><span class="stl_10 stl_08 stl_09">module</span><span class="stl_11 stl_08 stl_09">已经被启用。 &nbsp;</span></div>
                <div class="stl_01" style="top:52.961em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">4</span></div>
                <div class="stl_01" style="top:52.961em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">.7.1</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">、</span><span class="stl_40 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">nginx module </span><span class="stl_41 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">配置 &nbsp;</span></div>
                <div class="stl_01" style="top:55.7629em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:56.8884em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:58.0138em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:59.1393em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:60.2648em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:61.3903em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:62.5158em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:63.6413em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:55.7629em; left:6.8154em;"><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0001em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">module: nginx &nbsp;</span></div>
                <div class="stl_01" style="top:56.8884em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ</span><span class="stl_22 stl_08 stl_30" style="word-spacing:0.0001em;"># Access logs &nbsp;</span></div>
                <div class="stl_01" style="top:58.0138em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">access: &nbsp;</span></div>
                <div class="stl_01" style="top:59.1393em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ enabled:</span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0005em;"> true &nbsp;</span></div>
                <div class="stl_01" style="top:60.2648em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;">ꢀ var.paths:</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;"> [</span><span class="stl_29 stl_08 stl_09" style="word-spacing:0.0001em;">"/usr/local/nginx/logs/access.log*"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:62.5158em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.0001em;"># Set custom paths for the log files. If left empty, &nbsp;</span></div>
                <div class="stl_01" style="top:63.6413em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.0001em;"># Filebeat will choose the paths depending on your OS. &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_29.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_29.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.804em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:5.9295em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">10 &nbsp;</span></div>
                <div class="stl_01" style="top:7.055em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">11 &nbsp;</span></div>
                <div class="stl_01" style="top:8.1805em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">12 &nbsp;</span></div>
                <div class="stl_01" style="top:9.3059em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">13 &nbsp;</span></div>
                <div class="stl_01" style="top:10.4314em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">14 &nbsp;</span></div>
                <div class="stl_01" style="top:11.5569em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">15 &nbsp;</span></div>
                <div class="stl_01" style="top:12.6824em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">16 &nbsp;</span></div>
                <div class="stl_01" style="top:13.8079em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">17 &nbsp;</span></div>
                <div class="stl_01" style="top:14.9333em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">18 &nbsp;</span></div>
                <div class="stl_01" style="top:4.804em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ ꢀ</span><span class="stl_22 stl_08 stl_30" style="word-spacing:0.0002em;">#var.paths: &nbsp;</span></div>
                <div class="stl_01" style="top:7.055em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ</span><span class="stl_22 stl_08 stl_30" style="word-spacing:0.0001em;"># Error logs &nbsp;</span></div>
                <div class="stl_01" style="top:8.1805em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">error: &nbsp;</span></div>
                <div class="stl_01" style="top:9.3059em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ enabled:</span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0005em;"> true &nbsp;</span></div>
                <div class="stl_01" style="top:10.4314em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;">ꢀ var.paths:</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;"> [</span><span class="stl_29 stl_08 stl_09" style="word-spacing:0.0001em;">"/usr/local/nginx/logs/error.log*"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:12.6824em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.0001em;"># Set custom paths for the log files. If left empty, &nbsp;</span></div>
                <div class="stl_01" style="top:13.8079em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.0001em;"># Filebeat will choose the paths depending on your OS. &nbsp;</span></div>
                <div class="stl_01" style="top:14.9333em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ ꢀ</span><span class="stl_22 stl_08 stl_30" style="word-spacing:0.0002em;">#var.paths: &nbsp;</span></div>
                <div class="stl_01" style="top:17.5086em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">4</span></div>
                <div class="stl_01" style="top:17.5086em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">.7.2</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">、配置</span><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">ﬁlebeat &nbsp;</span></div>
                <div class="stl_01" style="top:20.3105em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:21.436em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:22.5615em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:23.687em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:24.8125em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:25.9379em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:27.0634em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:28.1889em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:29.3144em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:30.4399em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:20.3105em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">#vim itcast-nginx.yml &nbsp;</span></div>
                <div class="stl_01" style="top:22.5615em; left:6.8154em;"><span class="stl_27 stl_08 stl_30">filebeat.inputs</span><span class="stl_33 stl_08 stl_30">: &nbsp;</span></div>
                <div class="stl_01" style="top:23.687em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">#- type: log &nbsp;</span></div>
                <div class="stl_01" style="top:24.8125em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"># enabled:</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> true &nbsp;</span></div>
                <div class="stl_01" style="top:25.9379em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"># paths: &nbsp;</span></div>
                <div class="stl_01" style="top:27.0634em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"># ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"> -</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> /usr/local/nginx/logs/*.log &nbsp;</span></div>
                <div class="stl_01" style="top:28.1889em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"># tags:</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> ["nginx"] &nbsp;</span></div>
                <div class="stl_01" style="top:29.3144em; left:6.8154em;"><span class="stl_27 stl_08 stl_09">setup.template.settings</span><span class="stl_33 stl_08 stl_09">: &nbsp;</span></div>
                <div class="stl_01" style="top:30.4399em; left:7.6969em;"><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0004em;">index.number_of_shards</span><span class="stl_33 stl_08 stl_09" style="word-spacing:-0.0004em;">: </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0004em;">3 &nbsp;</span></div>
                <div class="stl_01" style="top:30.4399em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:31.5653em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:32.6908em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:33.8162em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:34.9417em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:36.0672em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:31.5653em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7646em;">1 </span><span class="stl_27 stl_08 stl_09" style="word-spacing:0.7646em;">output.elasticsearch</span><span class="stl_33 stl_08 stl_09" style="word-spacing:0.7646em;">: &nbsp;</span></div>
                <div class="stl_01" style="top:32.6908em; left:7.6969em;"><span class="stl_27 stl_08 stl_30" style="word-spacing:0.0001em;">hosts</span><span class="stl_33 stl_08 stl_30" style="word-spacing:0.0001em;">: [</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"192.168.40.133:9200"</span><span class="stl_33 stl_08 stl_30" style="word-spacing:0.0001em;">,</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"192.168.40.134:9200"</span><span class="stl_33 stl_08 stl_30" style="word-spacing:0.0001em;">,</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"192.168.40.135:9200"</span><span class="stl_33 stl_08 stl_30" style="word-spacing:0.0001em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:33.8162em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_27 stl_08 stl_09" style="word-spacing:0.7645em;">filebeat.config.modules</span><span class="stl_33 stl_08 stl_09" style="word-spacing:0.7645em;">: &nbsp;</span></div>
                <div class="stl_01" style="top:32.6908em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:34.9417em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:34.9417em; left:7.6969em;"><span class="stl_27 stl_08 stl_30" style="word-spacing:-0.0004em;">path</span><span class="stl_33 stl_08 stl_30" style="word-spacing:-0.0004em;">: </span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">$</span><span class="stl_33 stl_08 stl_30" style="word-spacing:-0.0004em;">{</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">path.config</span><span class="stl_33 stl_08 stl_30" style="word-spacing:-0.0004em;">}</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">/modules.d/*.yml &nbsp;</span></div>
                <div class="stl_01" style="top:36.0672em; left:7.6969em;"><span class="stl_27 stl_08 stl_30" style="word-spacing:-0.0004em;">reload.enabled</span><span class="stl_33 stl_08 stl_30" style="word-spacing:-0.0004em;">: </span><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0004em;">false &nbsp;</span></div>
                <div class="stl_01" style="top:36.0672em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:38.6425em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">4</span></div>
                <div class="stl_01" style="top:38.6425em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">.7.3</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">、测试 &nbsp;</span></div>
                <div class="stl_01" style="top:41.4444em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:42.5699em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:43.6954em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:44.8209em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:41.4444em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0008em;">./filebeat </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0008em;">-e -c </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0008em;">itcast-nginx.yml &nbsp;</span></div>
                <div class="stl_01" style="top:43.6954em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">启动会出错，如下 &nbsp;</span></div>
                <div class="stl_01" style="top:44.8209em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ERROR ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> fileset/factory.go:142</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;"> Error</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> loading pipeline:</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;"> Error loading pipeline</span><span class="stl_34 stl_08 stl_09" style="word-spacing:-0.0001em;"> for &nbsp;</span></div>
                <div class="stl_01" style="top:45.9464em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">fileset nginx/access: This module requires the following Elasticsearch plugins: &nbsp;</span></div>
                <div class="stl_01" style="top:47.0718em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ingest-user-agent, ingest-geoip. You can install them by running the following &nbsp;</span></div>
                <div class="stl_01" style="top:48.1973em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">commands on all the Elasticsearch nodes: &nbsp;</span></div>
                <div class="stl_01" style="top:49.3227em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:50.4482em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:51.5737em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:52.6991em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:53.8246em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:49.3227em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">ꢀ ꢀ</span><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.0002em;">sudo </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">bin/elasticsearch-plugin install ingest-user-agent &nbsp;</span></div>
                <div class="stl_01" style="top:50.4482em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">ꢀ ꢀ</span><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.0002em;">sudo </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">bin/elasticsearch-plugin install ingest-geoip &nbsp;</span></div>
                <div class="stl_01" style="top:51.5737em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ &nbsp;</span></div>
                <div class="stl_01" style="top:52.6991em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">解决：需要在</span><span class="stl_22 stl_08 stl_09">Elasticsearch</span><span class="stl_23 stl_08 stl_09">中安装</span><span class="stl_22 stl_08 stl_09">ingest-user-agent</span><span class="stl_23 stl_08 stl_09">、</span><span class="stl_22 stl_08 stl_09">ingest-geoip</span><span class="stl_23 stl_08 stl_09">插件 &nbsp;</span></div>
                <div class="stl_01" style="top:53.8246em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0em;">在资料中可以找到，</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">ingest-user-agent.tar</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0em;">、</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">ingest-geoip.tar</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0em;">、</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">ingest-geoip-conf.tar 3</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0em;">个文件 &nbsp;</span></div>
                <div class="stl_01" style="top:54.9501em; left:4.9337em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">10 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">其中，</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">ingest-user-agent.tar</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">、</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">ingest-geoip.tar</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">解压到</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">plugins</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">下 &nbsp;</span></div>
                <div class="stl_01" style="top:56.0756em; left:4.9337em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">11 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#ingest-geoip-conf.tar</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">解压到</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">config</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">下 &nbsp;</span></div>
                <div class="stl_01" style="top:57.2011em; left:4.9337em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">12 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">问题解决。 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_32.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_32.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:24.4316em; left:4.0017em;"><span class="stl_11 stl_08 stl_42">测试发现，数据已经写入到了</span><span class="stl_10 stl_08 stl_42">Elasticsearch</span><span class="stl_11 stl_08 stl_42">中，并且拿到的数据更加明确了： &nbsp;</span></div>
                <div class="stl_01" style="top:46.5034em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">当然了，其他的</span><span class="stl_10 stl_08 stl_09">Module</span><span class="stl_11 stl_08 stl_09">的用法参加官方文档： &nbsp;</span></div>
                <div class="stl_01" style="top:48.3792em; left:4.0017em;"><a href="https://www.elastic.co/guide/en/beats/filebeat/current/filebeat-modules.html" target="_blank"><span class="stl_25 stl_08 stl_26">https://www.elastic.co/guide/en/beats/ﬁlebeat/current/ﬁlebeat-modules.html &nbsp;</span></a></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_35.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_35.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:42.4912em; left:4.0017em;"><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">5</span><span class="stl_07 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">Metricbeat &nbsp;</span></div>
                <div class="stl_01" style="top:62.5102em; left:5.8775em;"><span class="stl_11 stl_08 stl_09">定期收集操作系统或应用服务的指标数据 &nbsp;</span></div>
                <div class="stl_01" style="top:63.7607em; left:5.8775em;"><span class="stl_11 stl_08 stl_38">存储到</span><span class="stl_10 stl_08 stl_38">Elasticsearch</span><span class="stl_11 stl_08 stl_38">中，进行实时分析 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_37.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_37.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.958em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">5</span></div>
                <div class="stl_01" style="top:4.958em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.1</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">Metricbeat</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">组成 &nbsp;</span></div>
                <div class="stl_01" style="top:7.4245em; left:4.0017em;"><span class="stl_10 stl_08 stl_09">Metricbeat</span><span class="stl_11 stl_08 stl_09">有</span><span class="stl_10 stl_08 stl_09">2</span><span class="stl_11 stl_08 stl_09">部分组成，一部分是</span><span class="stl_10 stl_08 stl_09">Module</span><span class="stl_11 stl_08 stl_09">，另一部分为</span><span class="stl_10 stl_08 stl_09">Metricset</span><span class="stl_11 stl_08 stl_09">。 &nbsp;</span></div>
                <div class="stl_01" style="top:9.3003em; left:5.8775em;"><span class="stl_10 stl_08 stl_09">Module &nbsp;</span></div>
                <div class="stl_01" style="top:10.9885em; left:7.7533em;"><span class="stl_11 stl_08 stl_35">收集的对象，如：</span><span class="stl_10 stl_08 stl_35">mysql</span><span class="stl_11 stl_08 stl_35">、</span><span class="stl_10 stl_08 stl_35">redis</span><span class="stl_11 stl_08 stl_35">、</span><span class="stl_10 stl_08 stl_35">nginx</span><span class="stl_11 stl_08 stl_35">、操作系统等； &nbsp;</span></div>
                <div class="stl_01" style="top:12.239em; left:5.8775em;"><span class="stl_10 stl_08 stl_09">Metricset &nbsp;</span></div>
                <div class="stl_01" style="top:13.8648em; left:7.7533em;"><span class="stl_11 stl_08 stl_09">收集指标的集合，如：</span><span class="stl_10 stl_08 stl_09">cpu</span><span class="stl_11 stl_08 stl_09">、</span><span class="stl_10 stl_08 stl_09">memory</span><span class="stl_11 stl_08 stl_09">、</span><span class="stl_10 stl_08 stl_09">network</span><span class="stl_11 stl_08 stl_09">等； &nbsp;</span></div>
                <div class="stl_01" style="top:15.8031em; left:4.0017em;"><span class="stl_11 stl_08 stl_09" style="word-spacing:0em;">以</span><span class="stl_10 stl_08 stl_09" style="word-spacing:0em;">Redis Module</span><span class="stl_11 stl_08 stl_09" style="word-spacing:0em;">为例： &nbsp;</span></div>
                <div class="stl_01" style="top:36.1587em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">5</span></div>
                <div class="stl_01" style="top:36.1587em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.2</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、部署与收集系统指标 &nbsp;</span></div>
                <div class="stl_01" style="top:39.1934em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:40.3189em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:41.4444em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:42.5699em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:43.6953em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:44.8208em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:45.9463em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:47.0718em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:48.1973em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:49.3227em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:39.1934em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">tar </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.001em;">-xvf </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">metricbeat-6.5.4-linux-x86_64.tar.gz &nbsp;</span></div>
                <div class="stl_01" style="top:40.3189em; left:6.8154em;"><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.0005em;">cd </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;">metricbeat-6.5.4-linux-x86_64 &nbsp;</span></div>
                <div class="stl_01" style="top:41.4444em; left:6.8154em;"><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.0007em;">vim </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0007em;">metricbeat.yml &nbsp;</span></div>
                <div class="stl_01" style="top:43.6953em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">metricbeat.config.modules: &nbsp;</span></div>
                <div class="stl_01" style="top:44.8208em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0006em;">path: </span><span class="stl_43 stl_08 stl_09" style="word-spacing:-0.0006em;">${path.config}</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0006em;">/modules.d/*.yml &nbsp;</span></div>
                <div class="stl_01" style="top:45.9463em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">reload.enabled: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0003em;">false &nbsp;</span></div>
                <div class="stl_01" style="top:47.0718em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">setup.template.settings: &nbsp;</span></div>
                <div class="stl_01" style="top:48.1973em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0009em;">index.number_of_shards: </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0009em;">1 &nbsp;</span></div>
                <div class="stl_01" style="top:49.3227em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">index.codec: best_compression &nbsp;</span></div>
                <div class="stl_01" style="top:49.3227em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:50.4482em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:51.5736em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:52.6991em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:53.8246em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:54.95em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:56.0755em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:57.201em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:58.3265em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:59.452em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:50.4482em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">setup.kibana: &nbsp;</span></div>
                <div class="stl_01" style="top:51.5736em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">output.elasticsearch: &nbsp;</span></div>
                <div class="stl_01" style="top:52.6991em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:52.6991em; left:7.6969em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">hosts: [</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"192.168.40.133:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">,</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"192.168.40.134:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">,</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"192.168.40.135:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:53.8246em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">processors: &nbsp;</span></div>
                <div class="stl_01" style="top:54.95em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:56.0755em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:57.201em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:54.95em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">ꢀ</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0001em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">add_host_metadata: ~ &nbsp;</span></div>
                <div class="stl_01" style="top:56.0755em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">ꢀ</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0001em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">add_cloud_metadata: ~ &nbsp;</span></div>
                <div class="stl_01" style="top:57.201em; left:7.2562em;"><span class="stl_19 stl_08 stl_09">ꢀ</span></div>
                <div class="stl_01" style="top:58.3265em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">8 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">启动 &nbsp;</span></div>
                <div class="stl_01" style="top:59.452em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">./metricbeat</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0005em;"> -e &nbsp;</span></div>
                <div class="stl_01" style="top:62.0725em; left:4.0017em;"><span class="stl_11 stl_08 stl_35">在</span><span class="stl_10 stl_08 stl_35">ELasticsearch</span><span class="stl_11 stl_08 stl_35">中可以看到，系统的一些指标数据已经写入进去了： &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_39.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_39.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:28.1208em; left:4.0017em;"><span class="stl_10 stl_08 stl_09" style="word-spacing:0em;">system module</span><span class="stl_11 stl_08 stl_09" style="word-spacing:0em;">配置： &nbsp;</span></div>
                <div class="stl_01" style="top:30.7524em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:31.8779em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:33.0034em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:30.7524em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">root@itcast01:modules.d# cat system.yml &nbsp;</span></div>
                <div class="stl_01" style="top:31.8779em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"># Module: system &nbsp;</span></div>
                <div class="stl_01" style="top:33.0034em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"># Docs: https://www.elastic.co/guide/en/beats/metricbeat/6.5/metricbeat-module- &nbsp;</span></div>
                <div class="stl_01" style="top:34.1288em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">system.html &nbsp;</span></div>
                <div class="stl_01" style="top:35.2543em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:36.3798em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:37.5053em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:38.6308em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:39.7562em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:40.8817em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:42.0072em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:43.1326em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:44.2581em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:45.3836em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:46.509em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:47.6345em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:48.76em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:49.8855em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:51.011em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:52.1364em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:53.2619em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:36.3798em; left:6.8154em;"><span class="stl_33 stl_08 stl_09" style="word-spacing:-0.0005em;">- </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0005em;">module</span><span class="stl_33 stl_08 stl_09" style="word-spacing:-0.0005em;">: </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;">system &nbsp;</span></div>
                <div class="stl_01" style="top:37.5053em; left:7.6969em;"><span class="stl_27 stl_08 stl_30" style="word-spacing:-0.0003em;">period</span><span class="stl_33 stl_08 stl_30" style="word-spacing:-0.0003em;">: </span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">10s &nbsp;</span></div>
                <div class="stl_01" style="top:38.6308em; left:7.6969em;"><span class="stl_27 stl_08 stl_09">metricsets</span><span class="stl_33 stl_08 stl_09">: &nbsp;</span></div>
                <div class="stl_01" style="top:39.7562em; left:7.2562em;"><span class="stl_33 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ -</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;"> cpu &nbsp;</span></div>
                <div class="stl_01" style="top:40.8817em; left:7.2562em;"><span class="stl_33 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ -</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;"> load &nbsp;</span></div>
                <div class="stl_01" style="top:42.0072em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:43.1326em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:44.2581em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:45.3836em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:46.509em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:47.6345em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:48.76em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:49.8855em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:51.011em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:52.1364em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:53.2619em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:54.3874em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:55.5129em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:56.6383em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:57.7637em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:58.8892em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:60.0147em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:61.1402em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:62.2657em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:63.3912em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:42.0072em; left:7.2562em;"><span class="stl_33 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ -</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;"> memory &nbsp;</span></div>
                <div class="stl_01" style="top:43.1326em; left:7.2562em;"><span class="stl_33 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ -</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;"> network &nbsp;</span></div>
                <div class="stl_01" style="top:44.2581em; left:7.2562em;"><span class="stl_33 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ -</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;"> process &nbsp;</span></div>
                <div class="stl_01" style="top:45.3836em; left:7.2562em;"><span class="stl_33 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ -</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;"> process_summary &nbsp;</span></div>
                <div class="stl_01" style="top:46.509em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0004em;">ꢀ ꢀ</span><span class="stl_22 stl_08 stl_31" style="word-spacing:0.0004em;">#- core &nbsp;</span></div>
                <div class="stl_01" style="top:47.6345em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0003em;">ꢀ ꢀ</span><span class="stl_22 stl_08 stl_30" style="word-spacing:0.0003em;">#- diskio &nbsp;</span></div>
                <div class="stl_01" style="top:48.76em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0003em;">ꢀ ꢀ</span><span class="stl_22 stl_08 stl_30" style="word-spacing:0.0003em;">#- socket &nbsp;</span></div>
                <div class="stl_01" style="top:49.8855em; left:7.6969em;"><span class="stl_27 stl_08 stl_09">process.include_top_n</span><span class="stl_33 stl_08 stl_09">: &nbsp;</span></div>
                <div class="stl_01" style="top:51.011em; left:7.2562em;"><span class="stl_27 stl_08 stl_30" style="word-spacing:0.6026em;">ꢀ by_cpu</span><span class="stl_33 stl_08 stl_30" style="word-spacing:0.6026em;">:</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;"> 5</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;"> ꢀ ꢀ ꢀ</span><span class="stl_22 stl_08 stl_30" style="word-spacing:0.0001em;"># include top 5 processes by</span><span class="stl_22 stl_08 stl_30" style="word-spacing:0.0001em;"> CPU &nbsp;</span></div>
                <div class="stl_01" style="top:52.1364em; left:7.2562em;"><span class="stl_27 stl_08 stl_09" style="word-spacing:0.6026em;">ꢀ by_memory</span><span class="stl_33 stl_08 stl_09" style="word-spacing:0.6026em;">:</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;"> 5</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;"> ꢀ </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0005em;">#</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> include</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> top 5</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> processes</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> by</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> memory &nbsp;</span></div>
                <div class="stl_01" style="top:54.3874em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_33 stl_08 stl_09" style="word-spacing:0.7645em;">-</span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0005em;"> module</span><span class="stl_33 stl_08 stl_09" style="word-spacing:-0.0005em;">:</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;"> system &nbsp;</span></div>
                <div class="stl_01" style="top:55.5129em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:56.6383em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:57.7637em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:58.8892em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:60.0147em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:61.1402em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:62.2657em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:63.3912em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:55.5129em; left:7.6969em;"><span class="stl_27 stl_08 stl_30" style="word-spacing:-0.0003em;">period</span><span class="stl_33 stl_08 stl_30" style="word-spacing:-0.0003em;">: </span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">1m &nbsp;</span></div>
                <div class="stl_01" style="top:56.6383em; left:7.6969em;"><span class="stl_27 stl_08 stl_09">metricsets</span><span class="stl_33 stl_08 stl_09">: &nbsp;</span></div>
                <div class="stl_01" style="top:57.7637em; left:7.2562em;"><span class="stl_33 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ -</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;"> filesystem &nbsp;</span></div>
                <div class="stl_01" style="top:58.8892em; left:7.2562em;"><span class="stl_33 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ -</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;"> fsstat &nbsp;</span></div>
                <div class="stl_01" style="top:60.0147em; left:7.6969em;"><span class="stl_27 stl_08 stl_09">processors</span><span class="stl_33 stl_08 stl_09">: &nbsp;</span></div>
                <div class="stl_01" style="top:61.1402em; left:7.6969em;"><span class="stl_33 stl_08 stl_30" style="word-spacing:-0.0008em;">- </span><span class="stl_27 stl_08 stl_30" style="word-spacing:-0.0008em;">drop_event.when.regexp</span><span class="stl_33 stl_08 stl_30" style="word-spacing:-0.0008em;">: &nbsp;</span></div>
                <div class="stl_01" style="top:62.2657em; left:7.2562em;"><span class="stl_27 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_27 stl_08 stl_09" style="word-spacing:0.6026em;"> system.filesystem.mount_point</span><span class="stl_33 stl_08 stl_09" style="word-spacing:0.6026em;">:</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0005em;"> '^/(sys|cgroup|proc|dev|etc|host|lib)($|/)' &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_40.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_40.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.8039em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:5.9294em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:7.0549em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:8.1804em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:9.3059em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:10.4314em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:11.5568em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:12.6823em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:13.8078em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:14.9333em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:4.8039em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_33 stl_08 stl_09" style="word-spacing:0.7645em;">-</span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0005em;"> module</span><span class="stl_33 stl_08 stl_09" style="word-spacing:-0.0005em;">:</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;"> system &nbsp;</span></div>
                <div class="stl_01" style="top:5.9294em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:7.0549em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:8.1804em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:9.3059em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:5.9294em; left:7.6969em;"><span class="stl_27 stl_08 stl_30" style="word-spacing:-0.0003em;">period</span><span class="stl_33 stl_08 stl_30" style="word-spacing:-0.0003em;">: </span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">15m &nbsp;</span></div>
                <div class="stl_01" style="top:7.0549em; left:7.6969em;"><span class="stl_27 stl_08 stl_09">metricsets</span><span class="stl_33 stl_08 stl_09">: &nbsp;</span></div>
                <div class="stl_01" style="top:8.1804em; left:7.2562em;"><span class="stl_33 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ -</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;"> uptime &nbsp;</span></div>
                <div class="stl_01" style="top:10.4314em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#-</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> module:</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> system &nbsp;</span></div>
                <div class="stl_01" style="top:11.5568em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">6 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"> period:</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> 5m &nbsp;</span></div>
                <div class="stl_01" style="top:12.6823em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">7 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"> metricsets: &nbsp;</span></div>
                <div class="stl_01" style="top:13.8078em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">8 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_22 stl_08 stl_09"> ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"> -</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> raid &nbsp;</span></div>
                <div class="stl_01" style="top:14.9333em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"> raid.mount_point:</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> '/' &nbsp;</span></div>
                <div class="stl_01" style="top:17.5884em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">5</span></div>
                <div class="stl_01" style="top:17.5884em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.3</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">Module &nbsp;</span></div>
                <div class="stl_01" style="top:20.6231em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:21.7486em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:22.8741em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:23.9996em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:25.125em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:26.2505em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:27.376em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:28.5015em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:29.6269em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:20.6231em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">./metricbeat modules list ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.0001em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.0001em;">查看列表 &nbsp;</span></div>
                <div class="stl_01" style="top:22.8741em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">Enabled: &nbsp;</span></div>
                <div class="stl_01" style="top:23.9996em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">system </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0004em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0004em;">默认启用 &nbsp;</span></div>
                <div class="stl_01" style="top:26.2505em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">Disabled: &nbsp;</span></div>
                <div class="stl_01" style="top:27.376em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">aerospike &nbsp;</span></div>
                <div class="stl_01" style="top:28.5015em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">apache &nbsp;</span></div>
                <div class="stl_01" style="top:29.6269em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">ceph &nbsp;</span></div>
                <div class="stl_01" style="top:30.7524em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:31.8778em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:33.0033em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:34.1288em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:35.2543em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:36.3798em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:37.5052em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:38.6307em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:39.7562em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:40.8817em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:42.0072em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:43.1326em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:44.2581em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:45.3835em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:46.509em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:47.6345em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:48.7599em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:49.8854em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:51.0109em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:52.1364em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:53.2619em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:54.3873em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:55.5128em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:56.6383em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:57.7637em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:58.8892em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:60.0147em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:61.1401em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:62.2656em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:63.3911em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:30.7524em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">couchbase &nbsp;</span></div>
                <div class="stl_01" style="top:31.8778em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">docker &nbsp;</span></div>
                <div class="stl_01" style="top:33.0033em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">dropwizard &nbsp;</span></div>
                <div class="stl_01" style="top:34.1288em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">elasticsearch &nbsp;</span></div>
                <div class="stl_01" style="top:35.2543em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">envoyproxy &nbsp;</span></div>
                <div class="stl_01" style="top:36.3798em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">etcd &nbsp;</span></div>
                <div class="stl_01" style="top:37.5052em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">6 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">golang &nbsp;</span></div>
                <div class="stl_01" style="top:38.6307em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">7 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">graphite &nbsp;</span></div>
                <div class="stl_01" style="top:39.7562em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">8 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">haproxy &nbsp;</span></div>
                <div class="stl_01" style="top:40.8817em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">http &nbsp;</span></div>
                <div class="stl_01" style="top:42.0072em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">jolokia &nbsp;</span></div>
                <div class="stl_01" style="top:43.1326em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">kafka &nbsp;</span></div>
                <div class="stl_01" style="top:44.2581em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">kibana &nbsp;</span></div>
                <div class="stl_01" style="top:45.3835em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">kubernetes &nbsp;</span></div>
                <div class="stl_01" style="top:46.509em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">kvm &nbsp;</span></div>
                <div class="stl_01" style="top:47.6345em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">logstash &nbsp;</span></div>
                <div class="stl_01" style="top:48.7599em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">6 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">memcached &nbsp;</span></div>
                <div class="stl_01" style="top:49.8854em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">7 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">mongodb &nbsp;</span></div>
                <div class="stl_01" style="top:51.0109em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">8 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">munin &nbsp;</span></div>
                <div class="stl_01" style="top:52.1364em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">mysql &nbsp;</span></div>
                <div class="stl_01" style="top:53.2619em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">nginx &nbsp;</span></div>
                <div class="stl_01" style="top:54.3873em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">php_fpm &nbsp;</span></div>
                <div class="stl_01" style="top:55.5128em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">postgresql &nbsp;</span></div>
                <div class="stl_01" style="top:56.6383em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">prometheus &nbsp;</span></div>
                <div class="stl_01" style="top:57.7637em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">rabbitmq &nbsp;</span></div>
                <div class="stl_01" style="top:58.8892em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">redis &nbsp;</span></div>
                <div class="stl_01" style="top:60.0147em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">6 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">traefik &nbsp;</span></div>
                <div class="stl_01" style="top:61.1401em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">7 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">uwsgi &nbsp;</span></div>
                <div class="stl_01" style="top:62.2656em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">8 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">vsphere &nbsp;</span></div>
                <div class="stl_01" style="top:63.3911em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">windows &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_42.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_42.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.804em; left:4.9337em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">40 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">zookeeper &nbsp;</span></div>
                <div class="stl_01" style="top:7.4592em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">5</span></div>
                <div class="stl_01" style="top:7.4592em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">.4</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">、</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">Nginx Module &nbsp;</span></div>
                <div class="stl_01" style="top:9.8803em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">5</span></div>
                <div class="stl_01" style="top:9.8803em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">.4.1</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">、开启</span><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">nginx</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">的状态查询 &nbsp;</span></div>
                <div class="stl_01" style="top:12.114em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">在</span><span class="stl_10 stl_08 stl_09">nginx</span><span class="stl_11 stl_08 stl_09">中，需要开启状态查询，才能查询到指标数据。 &nbsp;</span></div>
                <div class="stl_01" style="top:14.7457em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:15.8712em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:16.9967em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:18.1221em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:19.2476em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:20.373em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:21.4985em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:22.624em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:23.7495em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:24.875em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:14.7457em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">重新编译</span><span class="stl_22 stl_08 stl_09">nginx &nbsp;</span></div>
                <div class="stl_01" style="top:15.8712em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">./configure </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0001em;">--prefix</span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0001em;">=</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">/usr/local/nginx </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0001em;">--with-http_stub_status_module &nbsp;</span></div>
                <div class="stl_01" style="top:16.9967em; left:6.8154em;"><span class="stl_21 stl_08 stl_09">make &nbsp;</span></div>
                <div class="stl_01" style="top:18.1221em; left:6.8154em;"><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.001em;">make </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">install &nbsp;</span></div>
                <div class="stl_01" style="top:20.373em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;">./nginx </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0005em;">-V </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;">ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0005em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0005em;">查询版本信息 &nbsp;</span></div>
                <div class="stl_01" style="top:21.4985em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">nginx version: nginx/1.11.6 &nbsp;</span></div>
                <div class="stl_01" style="top:22.624em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0006em;">built by </span><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.0006em;">gcc </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0006em;">4</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0006em;">.4.7 </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0006em;">20120313 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0006em;">(Red Hat </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0006em;">4</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0006em;">.4.7-23) (GCC) &nbsp;</span></div>
                <div class="stl_01" style="top:23.7495em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">configure arguments: </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0004em;">--prefix</span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0004em;">=</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">/usr/local/nginx </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0004em;">--with-http_stub_status_module &nbsp;</span></div>
                <div class="stl_01" style="top:24.875em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:26.0004em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:27.1259em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:28.2514em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:29.3769em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:30.5024em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:31.6278em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:26.0004em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">配置</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">nginx &nbsp;</span></div>
                <div class="stl_01" style="top:27.1259em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_21 stl_08 stl_09" style="word-spacing:0.7645em;">vim</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0007em;"> nginx.conf &nbsp;</span></div>
                <div class="stl_01" style="top:28.2514em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">location</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> /nginx-status</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:29.3769em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:29.3769em; left:8.5778em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">stub_status on; &nbsp;</span></div>
                <div class="stl_01" style="top:30.5024em; left:8.5778em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">access_log off; &nbsp;</span></div>
                <div class="stl_01" style="top:30.5024em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:31.6278em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">6 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:34.2483em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">测试： &nbsp;</span></div>
                <div class="stl_01" style="top:45.9408em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">结果说明： &nbsp;</span></div>
                <div class="stl_01" style="top:47.8165em; left:5.8775em;"><span class="stl_10 stl_08 stl_09" style="word-spacing:0em;">Active connections</span><span class="stl_11 stl_08 stl_09" style="word-spacing:0em;">：正在处理的活动连接数 &nbsp;</span></div>
                <div class="stl_01" style="top:49.5047em; left:5.8775em;"><span class="stl_10 stl_08 stl_26" style="word-spacing:0.0017em;">server accepts handled requests &nbsp;</span></div>
                <div class="stl_01" style="top:51.1304em; left:7.7533em;"><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0049em;">第一个 </span><span class="stl_10 stl_08 stl_09" style="word-spacing:0.0049em;">server </span><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0049em;">表示</span><span class="stl_10 stl_08 stl_09" style="word-spacing:0.0049em;">Nginx</span><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0049em;">启动到现在共处理了</span><span class="stl_10 stl_08 stl_09" style="word-spacing:0.0049em;">9</span><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0049em;">个连接 &nbsp;</span></div>
                <div class="stl_01" style="top:52.3809em; left:7.7533em;"><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0049em;">第二个 </span><span class="stl_10 stl_08 stl_09" style="word-spacing:0.0049em;">accepts </span><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0049em;">表示</span><span class="stl_10 stl_08 stl_09" style="word-spacing:0.0049em;">Nginx</span><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0049em;">启动到现在共成功创建 </span><span class="stl_10 stl_08 stl_09" style="word-spacing:0.0049em;">9 </span><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0049em;">次握手 &nbsp;</span></div>
                <div class="stl_01" style="top:53.6314em; left:7.7533em;"><span class="stl_11 stl_08 stl_26" style="word-spacing:0.0056em;">第三个 </span><span class="stl_10 stl_08 stl_26" style="word-spacing:0.0056em;">handled requests </span><span class="stl_11 stl_08 stl_26" style="word-spacing:0.0056em;">表示总共处理了 </span><span class="stl_10 stl_08 stl_26" style="word-spacing:0.0056em;">21 </span><span class="stl_11 stl_08 stl_26" style="word-spacing:0.0056em;">次请求 &nbsp;</span></div>
                <div class="stl_01" style="top:54.882em; left:7.7533em;"><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0059em;">请求丢失数 </span><span class="stl_10 stl_08 stl_09" style="word-spacing:0.0059em;">= </span><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0059em;">握手数 </span><span class="stl_10 stl_08 stl_09" style="word-spacing:0.0059em;">- </span><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0059em;">连接数 ，可以看出目前为止没有丢失请求 &nbsp;</span></div>
                <div class="stl_01" style="top:56.1325em; left:5.8775em;"><span class="stl_10 stl_08 stl_24" style="word-spacing:0.0028em;">Reading: 0 Writing: 1 Waiting: 1 &nbsp;</span></div>
                <div class="stl_01" style="top:57.8207em; left:7.7533em;"><span class="stl_10 stl_08 stl_09" style="word-spacing:0.0033em;">Reading</span><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0033em;">：</span><span class="stl_10 stl_08 stl_09" style="word-spacing:0.0033em;">Nginx </span><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0033em;">读取到客户端的 </span><span class="stl_10 stl_08 stl_09" style="word-spacing:0.0033em;">Header </span><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0033em;">信息数 &nbsp;</span></div>
                <div class="stl_01" style="top:59.0712em; left:7.7533em;"><span class="stl_10 stl_08 stl_45" style="word-spacing:0.0041em;">Writing</span><span class="stl_11 stl_08 stl_45" style="word-spacing:0.0041em;">：</span><span class="stl_10 stl_08 stl_45" style="word-spacing:0.0041em;">Nginx </span><span class="stl_11 stl_08 stl_45" style="word-spacing:0.0041em;">返回给客户端 </span><span class="stl_10 stl_08 stl_45" style="word-spacing:0.0041em;">Header </span><span class="stl_11 stl_08 stl_45" style="word-spacing:0.0041em;">信息数 &nbsp;</span></div>
                <div class="stl_01" style="top:60.3218em; left:7.7533em;"><span class="stl_10 stl_08 stl_15" style="word-spacing:0.0015em;">Waiting</span><span class="stl_11 stl_08 stl_15" style="word-spacing:0.0015em;">：</span><span class="stl_10 stl_08 stl_15" style="word-spacing:0.0015em;">Nginx </span><span class="stl_11 stl_08 stl_15" style="word-spacing:0.0015em;">已经处理完正在等候下一次请求指令的驻留链接（开启</span><span class="stl_10 stl_08 stl_15" style="word-spacing:0.0015em;">keep-alive</span><span class="stl_11 stl_08 stl_15" style="word-spacing:0.0015em;">的情况下，这个值等于 &nbsp;</span></div>
                <div class="stl_01" style="top:61.5723em; left:7.7533em;"><span class="stl_10 stl_08 stl_45" style="word-spacing:0.0009em;">Active - (Reading+Writing)</span><span class="stl_11 stl_08 stl_45" style="word-spacing:0.0009em;">） &nbsp;</span></div>
                <div class="stl_01" style="top:63.5905em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">5</span></div>
                <div class="stl_01" style="top:63.5905em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">.4.2</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">、配置</span><span class="stl_40 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">Nginx Module &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_43.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_43.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:5.3667em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:6.4922em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:7.6177em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:8.7432em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:9.8686em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:10.9941em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:12.1195em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:13.245em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:5.3667em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0em;">启用</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">redis module &nbsp;</span></div>
                <div class="stl_01" style="top:6.4922em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">./metricbeat modules enable nginx &nbsp;</span></div>
                <div class="stl_01" style="top:8.7432em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0em;">修改</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">redis module</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0em;">配置 &nbsp;</span></div>
                <div class="stl_01" style="top:9.8686em; left:6.8154em;"><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.0007em;">vim </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0007em;">modules.d/nginx.yml &nbsp;</span></div>
                <div class="stl_01" style="top:12.1195em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"># Module: nginx &nbsp;</span></div>
                <div class="stl_01" style="top:13.245em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"># Docs: https://www.elastic.co/guide/en/beats/metricbeat/6.5/metricbeat-module- &nbsp;</span></div>
                <div class="stl_01" style="top:14.3705em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">nginx.html &nbsp;</span></div>
                <div class="stl_01" style="top:15.496em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:16.6214em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:17.7469em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:18.8724em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:19.9979em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:21.1234em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:22.2488em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:23.3743em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:24.4998em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:25.6252em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:26.7507em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:27.8762em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:29.0016em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:30.1271em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:31.2526em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:32.3781em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:33.5036em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:34.629em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:16.6214em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_20 stl_08 stl_09" style="word-spacing:0.7645em;">-</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;"> module:</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> nginx &nbsp;</span></div>
                <div class="stl_01" style="top:17.7469em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:18.8724em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:19.9979em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:21.1234em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:22.2488em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:23.3743em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:24.4998em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:25.6252em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:26.7507em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:27.8762em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:29.0016em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:30.1271em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:31.2526em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:32.3781em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:17.7469em; left:7.2562em;"><span class="stl_19 stl_08 stl_09">ꢀ</span><span class="stl_22 stl_08 stl_09">#metricsets: &nbsp;</span></div>
                <div class="stl_01" style="top:18.8724em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;">ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6026em;"># -</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.0001em;"> stubstatus &nbsp;</span></div>
                <div class="stl_01" style="top:19.9979em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">period: 10s &nbsp;</span></div>
                <div class="stl_01" style="top:22.2488em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ</span><span class="stl_22 stl_08 stl_30" style="word-spacing:0.0001em;"># Nginx hosts &nbsp;</span></div>
                <div class="stl_01" style="top:23.3743em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">hosts: [</span><span class="stl_29 stl_08 stl_09" style="word-spacing:0.0001em;">"http://192.168.40.133"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:25.6252em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"># Path to server status. Default server-status &nbsp;</span></div>
                <div class="stl_01" style="top:26.7507em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0013em;">server_status_path: </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0013em;">"nginx-status" &nbsp;</span></div>
                <div class="stl_01" style="top:29.0016em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.0001em;">#username: "user" &nbsp;</span></div>
                <div class="stl_01" style="top:30.1271em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.0001em;">#password: "secret" &nbsp;</span></div>
                <div class="stl_01" style="top:33.5036em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">启动 &nbsp;</span></div>
                <div class="stl_01" style="top:34.629em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">6 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">./metricbeat</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0005em;"> -e &nbsp;</span></div>
                <div class="stl_01" style="top:37.2495em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">测试： &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_46.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_46.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:42.1892em; left:4.0017em;"><span class="stl_11 stl_08 stl_35">可以看到，</span><span class="stl_10 stl_08 stl_35">nginx</span><span class="stl_11 stl_08 stl_35">的指标数据已经写入到了</span><span class="stl_10 stl_08 stl_35">Elasticsearch</span><span class="stl_11 stl_08 stl_35">。 &nbsp;</span></div>
                <div class="stl_01" style="top:44.1275em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">更多的</span><span class="stl_10 stl_08 stl_09">Module</span><span class="stl_11 stl_08 stl_09">使用参见官方文档： &nbsp;</span></div>
                <div class="stl_01" style="top:46.0032em; left:4.0017em;"><a href="https://www.elastic.co/guide/en/beats/metricbeat/current/metricbeat-modules.html" target="_blank"><span class="stl_25 stl_08 stl_26">https://www.elastic.co/guide/en/beats/metricbeat/current/metricbeat-modules.html &nbsp;</span></a></div>
                <div class="stl_01" style="top:47.9935em; left:4.0017em;"><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">6</span><span class="stl_07 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">Kibana &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_48.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_48.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.9234em; left:4.0017em;"><span class="stl_10 stl_08 stl_37" style="word-spacing:0.0039em;">Kibana </span><span class="stl_11 stl_08 stl_37" style="word-spacing:0.0039em;">是一款开源的数据分析和可视化平台，它是 </span><span class="stl_10 stl_08 stl_37" style="word-spacing:0.0039em;">Elastic Stack </span><span class="stl_11 stl_08 stl_37" style="word-spacing:0.0039em;">成员之一，设计用于和 </span><span class="stl_10 stl_08 stl_37" style="word-spacing:0.0039em;">Elasticsearch </span><span class="stl_11 stl_08 stl_37" style="word-spacing:0.0039em;">协作。您可以 &nbsp;</span></div>
                <div class="stl_01" style="top:6.1739em; left:4.0017em;"><span class="stl_11 stl_08 stl_45" style="word-spacing:0.0056em;">使用 </span><span class="stl_10 stl_08 stl_45" style="word-spacing:0.0056em;">Kibana </span><span class="stl_11 stl_08 stl_45" style="word-spacing:0.0056em;">对 </span><span class="stl_10 stl_08 stl_45" style="word-spacing:0.0056em;">Elasticsearch </span><span class="stl_11 stl_08 stl_45" style="word-spacing:0.0056em;">索引中的数据进行搜索、查看、交互操作。您可以很方便的利用图表、表格及地图对 &nbsp;</span></div>
                <div class="stl_01" style="top:7.4246em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">数据进行多元化的分析和呈现。 &nbsp;</span></div>
                <div class="stl_01" style="top:9.3002em; left:4.0017em;"><span class="stl_11 stl_08 stl_24">官网：</span><a href="https://www.elastic.co/cn/products/kibana" target="_blank"><span class="stl_25 stl_08 stl_24">https://www.elastic.co/cn/products/kibana &nbsp;</span></a></div>
                <div class="stl_01" style="top:11.3983em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">6</span></div>
                <div class="stl_01" style="top:11.3983em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.1</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、配置安装 &nbsp;</span></div>
                <div class="stl_01" style="top:14.4331em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:15.5584em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:16.6839em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:17.8094em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:18.9349em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:20.0604em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:21.1859em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:22.3114em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:23.4368em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:14.4331em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">解压安装包 &nbsp;</span></div>
                <div class="stl_01" style="top:15.5584em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">tar </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.001em;">-xvf </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">kibana-6.5.4-linux-x86_64.tar.gz &nbsp;</span></div>
                <div class="stl_01" style="top:17.8094em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">修改配置文件 &nbsp;</span></div>
                <div class="stl_01" style="top:18.9349em; left:6.8154em;"><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.0007em;">vim </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0007em;">config/kibana.yml &nbsp;</span></div>
                <div class="stl_01" style="top:21.1859em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0008em;">server.host: </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0008em;">"192.168.40.133" </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0008em;">ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0008em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0008em;">对外暴露服务的地址 &nbsp;</span></div>
                <div class="stl_01" style="top:22.3114em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">elasticsearch.url: </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0003em;">"http://192.168.40.133:9200" </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0003em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0003em;">配置</span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0003em;">Elasticsearch &nbsp;</span></div>
                <div class="stl_01" style="top:24.5623em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:25.6878em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:26.8131em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:27.9386em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:29.0641em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:24.5623em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">启动 &nbsp;</span></div>
                <div class="stl_01" style="top:25.6878em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">./bin/kibana &nbsp;</span></div>
                <div class="stl_01" style="top:26.8131em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:27.9386em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">通过浏览器进行访问 &nbsp;</span></div>
                <div class="stl_01" style="top:29.0641em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">http://192.168.40.133:5601/app/kibana &nbsp;</span></div>
                <div class="stl_01" style="top:51.6931em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">可以看到</span><span class="stl_10 stl_08 stl_09">kibana</span><span class="stl_11 stl_08 stl_09">页面，并且可以看到提示，导入数据到</span><span class="stl_10 stl_08 stl_09">Kibana</span><span class="stl_11 stl_08 stl_09">。 &nbsp;</span></div>
                <div class="stl_01" style="top:53.7911em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">6</span></div>
                <div class="stl_01" style="top:53.7911em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.2</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、功能说明 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_50.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_50.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:41.2234em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">6</span></div>
                <div class="stl_01" style="top:41.2234em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.3</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、数据探索 &nbsp;</span></div>
                <div class="stl_01" style="top:43.6899em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">首先先添加索引信息： &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_53.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_53.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:30.6218em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">即可查看索引数据： &nbsp;</span></div>
                <div class="stl_01" style="top:55.9795em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">6</span></div>
                <div class="stl_01" style="top:55.9795em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">.4</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">、</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">Metricbeat </span><span class="stl_14 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">仪表盘 &nbsp;</span></div>
                <div class="stl_01" style="top:58.446em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">可以将</span><span class="stl_10 stl_08 stl_09">Metricbeat</span><span class="stl_11 stl_08 stl_09">的数据在</span><span class="stl_10 stl_08 stl_09">Kibana</span><span class="stl_11 stl_08 stl_09">中展示。 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_55.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_55.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:5.3667em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:6.4922em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:7.6177em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:8.7432em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:9.8686em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:10.9941em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:12.1196em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:5.3667em; left:6.3152em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">修改</span><span class="stl_22 stl_08 stl_09">metricbeat</span><span class="stl_23 stl_08 stl_09">配置 &nbsp;</span></div>
                <div class="stl_01" style="top:6.4922em; left:6.3152em;"><span class="stl_19 stl_08 stl_09">setup.kibana: &nbsp;</span></div>
                <div class="stl_01" style="top:7.6177em; left:7.1967em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0006em;">host: </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0006em;">"192.168.40.133:5601" &nbsp;</span></div>
                <div class="stl_01" style="top:8.7432em; left:6.7559em;"><span class="stl_19 stl_08 stl_09">ꢀ</span></div>
                <div class="stl_01" style="top:9.8686em; left:6.3152em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">安装仪表盘到</span><span class="stl_22 stl_08 stl_09">Kibana &nbsp;</span></div>
                <div class="stl_01" style="top:10.9941em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">./metricbeat setup </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0003em;">--dashboards &nbsp;</span></div>
                <div class="stl_01" style="top:14.7402em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">即可在</span><span class="stl_10 stl_08 stl_09">Kibana</span><span class="stl_11 stl_08 stl_09">中看到仪表盘数据： &nbsp;</span></div>
                <div class="stl_01" style="top:42.8769em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">查看系统信息： &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_58.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_58.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:28.5305em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">6</span></div>
                <div class="stl_01" style="top:28.5305em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">.5</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">、</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">Nginx </span><span class="stl_14 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">指标仪表盘 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_60.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_60.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:40.0354em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">6</span></div>
                <div class="stl_01" style="top:40.0354em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">.6</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">、</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">Nginx </span><span class="stl_14 stl_08 stl_09" style="font-weight:bold; word-spacing:0em;">日志仪表盘 &nbsp;</span></div>
                <div class="stl_01" style="top:43.0701em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:44.1956em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:45.3211em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:46.4466em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:47.5721em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:48.6976em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:49.8229em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:50.9484em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:52.0739em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:43.0701em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0.3525em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.3525em;">修改配置文件 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.3525em;">vim</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> itcast-nginx.yml &nbsp;</span></div>
                <div class="stl_01" style="top:44.1956em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">filebeat.inputs: &nbsp;</span></div>
                <div class="stl_01" style="top:45.3211em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">#- type: log &nbsp;</span></div>
                <div class="stl_01" style="top:46.4466em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"># enabled:</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> true &nbsp;</span></div>
                <div class="stl_01" style="top:47.5721em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"># paths: &nbsp;</span></div>
                <div class="stl_01" style="top:48.6976em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"># ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"> -</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> /usr/local/nginx/logs/*.log &nbsp;</span></div>
                <div class="stl_01" style="top:49.8229em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"># tags:</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> ["nginx"] &nbsp;</span></div>
                <div class="stl_01" style="top:50.9484em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">setup.template.settings: &nbsp;</span></div>
                <div class="stl_01" style="top:52.0739em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0009em;">index.number_of_shards: </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0009em;">3 &nbsp;</span></div>
                <div class="stl_01" style="top:53.1994em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:54.3249em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:55.4504em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:56.5758em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:57.7013em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:58.8268em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:59.9523em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:61.0778em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:62.2031em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:63.3286em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:53.1994em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">output.elasticsearch: &nbsp;</span></div>
                <div class="stl_01" style="top:54.3249em; left:7.6969em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">hosts: [</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"192.168.40.133:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">,</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"192.168.40.134:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">,</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"192.168.40.135:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:55.4504em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">filebeat.config.modules: &nbsp;</span></div>
                <div class="stl_01" style="top:54.3249em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:56.5758em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:57.7013em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:56.5758em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0006em;">path: </span><span class="stl_43 stl_08 stl_09" style="word-spacing:-0.0006em;">${path.config}</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0006em;">/modules.d/*.yml &nbsp;</span></div>
                <div class="stl_01" style="top:57.7013em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">reload.enabled: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0003em;">false &nbsp;</span></div>
                <div class="stl_01" style="top:58.8268em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">setup.kibana: &nbsp;</span></div>
                <div class="stl_01" style="top:59.9523em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:61.0778em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:62.2031em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:59.9523em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0006em;">host: </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0006em;">"192.168.40.133:5601" &nbsp;</span></div>
                <div class="stl_01" style="top:62.2031em; left:7.2562em;"><span class="stl_19 stl_08 stl_09">ꢀ</span></div>
                <div class="stl_01" style="top:63.3286em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">安装仪表盘到</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">kibana &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_63.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_63.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.804em; left:4.9337em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">20 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">./filebeat</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0013em;"> -c</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;"> itcast-nginx.yml</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> setup &nbsp;</span></div>
                <div class="stl_01" style="top:7.4246em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">可以看到</span><span class="stl_10 stl_08 stl_09">nginx</span><span class="stl_11 stl_08 stl_09">的</span><span class="stl_10 stl_08 stl_09">FileBeat</span><span class="stl_11 stl_08 stl_09">的仪表盘了： &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_66.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_66.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:26.342em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">6</span></div>
                <div class="stl_01" style="top:26.342em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.7</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、自定义图表 &nbsp;</span></div>
                <div class="stl_01" style="top:28.8085em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">在</span><span class="stl_10 stl_08 stl_09">Kibana</span><span class="stl_11 stl_08 stl_09">中，也可以进行自定义图表，如制作柱形图： &nbsp;</span></div>
                <div class="stl_01" style="top:50.6301em; left:4.0017em;"><span class="stl_11 stl_08 stl_32">将图表添加到自定义</span><span class="stl_10 stl_08 stl_32">Dashboard</span><span class="stl_11 stl_08 stl_32">中： &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_70.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_70.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:24.4662em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">6</span></div>
                <div class="stl_01" style="top:24.4662em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.8</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、开发者工具 &nbsp;</span></div>
                <div class="stl_01" style="top:26.9327em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">在</span><span class="stl_10 stl_08 stl_09">Kibana</span><span class="stl_11 stl_08 stl_09">中，为开发者的测试提供了便捷的工具使用，如下： &nbsp;</span></div>
                <div class="stl_01" style="top:43.8042em; left:4.0017em;"><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">7</span><span class="stl_07 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">Logstash &nbsp;</span></div>
                <div class="stl_01" style="top:46.8506em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">7</span></div>
                <div class="stl_01" style="top:46.8506em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.1</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、简介 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_73.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_73.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.9236em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">用途： &nbsp;</span></div>
                <div class="stl_01" style="top:30.4063em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">7</span></div>
                <div class="stl_01" style="top:30.4063em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.2</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、部署安装 &nbsp;</span></div>
                <div class="stl_01" style="top:43.5703em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:44.6958em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:45.8213em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:46.9468em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:48.0723em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:49.1977em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:50.3232em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:51.4487em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:43.5703em; left:6.3152em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">检查</span><span class="stl_22 stl_08 stl_09">jdk</span><span class="stl_23 stl_08 stl_09">环境，要求</span><span class="stl_22 stl_08 stl_09">jdk1.8+ &nbsp;</span></div>
                <div class="stl_01" style="top:44.6958em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0012em;">java </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0012em;">-version &nbsp;</span></div>
                <div class="stl_01" style="top:46.9468em; left:6.3152em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">解压安装包 &nbsp;</span></div>
                <div class="stl_01" style="top:48.0723em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">tar </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.001em;">-xvf </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">logstash-6.5.4.tar.gz &nbsp;</span></div>
                <div class="stl_01" style="top:50.3232em; left:6.3152em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">第一个</span><span class="stl_22 stl_08 stl_09">logstash</span><span class="stl_23 stl_08 stl_09">示例 &nbsp;</span></div>
                <div class="stl_01" style="top:51.4487em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">bin/logstash </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0001em;">-e </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0001em;">'input { stdin { } } output { stdout {} }' &nbsp;</span></div>
                <div class="stl_01" style="top:54.0693em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">执行效果如下： &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_76.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_76.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:20.9649em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">7</span></div>
                <div class="stl_01" style="top:20.9649em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.3</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、配置详解 &nbsp;</span></div>
                <div class="stl_01" style="top:23.4312em; left:4.0017em;"><span class="stl_10 stl_08 stl_09">Logstash</span><span class="stl_11 stl_08 stl_09">的配置有三部分，如下： &nbsp;</span></div>
                <div class="stl_01" style="top:26.063em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:27.1885em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:28.314em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:29.4394em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:30.5648em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:31.6903em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:32.8158em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:33.9412em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:35.0667em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:36.1922em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:26.063em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">input { </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0003em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0003em;">输入 &nbsp;</span></div>
                <div class="stl_01" style="top:27.1885em; left:8.5778em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">stdin { ... } </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0002em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0002em;">标准输入 &nbsp;</span></div>
                <div class="stl_01" style="top:28.314em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">}</span></div>
                <div class="stl_01" style="top:30.5648em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">filter { </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0004em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0004em;">过滤，对数据进行分割、截取等处理 &nbsp;</span></div>
                <div class="stl_01" style="top:31.6903em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ ... &nbsp;</span></div>
                <div class="stl_01" style="top:32.8158em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">}</span></div>
                <div class="stl_01" style="top:35.0667em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">output { </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0004em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0004em;">输出 &nbsp;</span></div>
                <div class="stl_01" style="top:36.1922em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:37.3177em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:36.1922em; left:8.5778em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">stdout { ... } </span><span class="stl_22 stl_08 stl_09" style="word-spacing:-0.0002em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:-0.0002em;">标准输出 &nbsp;</span></div>
                <div class="stl_01" style="top:37.3177em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:39.893em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">7</span></div>
                <div class="stl_01" style="top:39.893em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">.3.1</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">、输入 &nbsp;</span></div>
                <div class="stl_01" style="top:42.1265em; left:5.8775em;"><span class="stl_11 stl_08 stl_09">采集各种样式、大小和来源的数据，数据往往以各种各样的形式，或分散或集中地存在于很多系统中。 &nbsp;</span></div>
                <div class="stl_01" style="top:43.3772em; left:5.8775em;"><span class="stl_10 stl_08 stl_09" style="word-spacing:0.0049em;">Logstash </span><span class="stl_11 stl_08 stl_09" style="word-spacing:0.0049em;">支持各种输入选择 ，可以在同一时间从众多常用来源捕捉事件。能够以连续的流式传输方式，轻松地 &nbsp;</span></div>
                <div class="stl_01" style="top:44.6277em; left:5.8775em;"><span class="stl_11 stl_08 stl_46" style="word-spacing:0.0074em;">从您的日志、指标、</span><span class="stl_10 stl_08 stl_46" style="word-spacing:0.0074em;">Web </span><span class="stl_11 stl_08 stl_46" style="word-spacing:0.0074em;">应用、数据存储以及各种 </span><span class="stl_10 stl_08 stl_46" style="word-spacing:0.0074em;">AWS </span><span class="stl_11 stl_08 stl_46" style="word-spacing:0.0074em;">服务采集数据。 &nbsp;</span></div>
                <div class="stl_01" style="top:62.9027em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">7</span></div>
                <div class="stl_01" style="top:62.9027em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">.3.2</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">、过滤 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_79.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_79.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.9234em; left:5.8775em;"><span class="stl_11 stl_08 stl_09">实时解析和转换数据 &nbsp;</span></div>
                <div class="stl_01" style="top:6.1739em; left:5.8775em;"><span class="stl_11 stl_08 stl_09" style="word-spacing:0em;">数据从源传输到存储库的过程中，</span><span class="stl_10 stl_08 stl_09" style="word-spacing:0em;">Logstash </span><span class="stl_11 stl_08 stl_09" style="word-spacing:0em;">过滤器能够解析各个事件，识别已命名的字段以构建结构，并将它 &nbsp;</span></div>
                <div class="stl_01" style="top:7.4246em; left:5.8775em;"><span class="stl_11 stl_08 stl_09">们转换成通用格式，以便更轻松、更快速地分析和实现商业价值。 &nbsp;</span></div>
                <div class="stl_01" style="top:32.0147em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">7</span></div>
                <div class="stl_01" style="top:32.0147em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">.3.3</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">、输出 &nbsp;</span></div>
                <div class="stl_01" style="top:34.2483em; left:4.0017em;"><span class="stl_10 stl_08 stl_09" style="word-spacing:0em;">Logstash </span><span class="stl_11 stl_08 stl_09" style="word-spacing:0em;">提供众多输出选择，您可以将数据发送到您要指定的地方，并且能够灵活地解锁众多下游用例。 &nbsp;</span></div>
                <div class="stl_01" style="top:52.6656em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">7</span></div>
                <div class="stl_01" style="top:52.6656em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.4</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、读取自定义日志 &nbsp;</span></div>
                <div class="stl_01" style="top:55.1321em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">前面我们通过</span><span class="stl_10 stl_08 stl_09">Filebeat</span><span class="stl_11 stl_08 stl_09">读取了</span><span class="stl_10 stl_08 stl_09">nginx</span><span class="stl_11 stl_08 stl_09">的日志，如果是自定义结构的日志，就需要读取处理后才能使用，所以，这个时 &nbsp;</span></div>
                <div class="stl_01" style="top:56.3826em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">候就需要使用</span><span class="stl_10 stl_08 stl_09">Logstash</span><span class="stl_11 stl_08 stl_09">了，因为</span><span class="stl_10 stl_08 stl_09">Logstash</span><span class="stl_11 stl_08 stl_09">有着强大的处理能力，可以应对各种各样的场景。 &nbsp;</span></div>
                <div class="stl_01" style="top:58.4008em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">7</span></div>
                <div class="stl_01" style="top:58.4008em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">.4.1</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">、日志结构 &nbsp;</span></div>
                <div class="stl_01" style="top:61.2026em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:61.2026em; left:6.3152em;"><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0002em;">2019</span><span class="stl_20 stl_08 stl_30" style="word-spacing:-0.0002em;">-03-15 </span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0002em;">21</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">:21:21|ERROR|</span><span class="stl_39 stl_08 stl_30" style="word-spacing:-0.0002em;">读取数据出错</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">|</span><span class="stl_39 stl_08 stl_30" style="word-spacing:-0.0002em;">参数</span><span class="stl_47 stl_08 stl_30" style="word-spacing:-0.0002em;">：</span><span class="stl_43 stl_08 stl_30" style="word-spacing:-0.0002em;">id</span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0002em;">=</span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0002em;">1002 &nbsp;</span></div>
                <div class="stl_01" style="top:63.8232em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">可以看到，日志中的内容是使用</span><span class="stl_10 stl_08 stl_09">“|”</span><span class="stl_11 stl_08 stl_09">进行分割的，使用，我们在处理的时候，也需要对数据做分割处理。 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_80.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_80.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.8783em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">7</span></div>
                <div class="stl_01" style="top:4.8783em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">.4.2</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">、编写配置文件 &nbsp;</span></div>
                <div class="stl_01" style="top:7.6803em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:8.8058em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:9.9313em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:11.0568em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:12.1821em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:13.3076em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:14.4331em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:15.5586em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:16.6841em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:7.6803em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">#vim itcast-pipeline.conf &nbsp;</span></div>
                <div class="stl_01" style="top:9.9313em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">input { &nbsp;</span></div>
                <div class="stl_01" style="top:11.0568em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ file { &nbsp;</span></div>
                <div class="stl_01" style="top:12.1821em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;"> path</span><span class="stl_44 stl_08 stl_09" style="word-spacing:0.6026em;"> =</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0013em;">&gt;</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0005em;"> "/itcast/logstash/logs/app.log" &nbsp;</span></div>
                <div class="stl_01" style="top:13.3076em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;"> start_position</span><span class="stl_44 stl_08 stl_09" style="word-spacing:0.6026em;"> =</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">&gt;</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0005em;"> "beginning" &nbsp;</span></div>
                <div class="stl_01" style="top:14.4331em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ } &nbsp;</span></div>
                <div class="stl_01" style="top:15.5586em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">}</span></div>
                <div class="stl_01" style="top:17.8096em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:18.9351em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:20.0605em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:21.186em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:22.3115em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:23.4368em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:24.5623em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:25.6878em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:26.8133em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:17.8096em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">filter</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:18.9351em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:18.9351em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ mutate</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:20.0605em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:20.0605em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">ꢀ ꢀ</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.6028em;"> split</span><span class="stl_44 stl_08 stl_31" style="word-spacing:0.6028em;"> =</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">&gt;</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;"> {</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0003em;">"message"</span><span class="stl_44 stl_08 stl_31" style="word-spacing:0.0003em;">=</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">&gt;</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0003em;">"|"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:21.186em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ } &nbsp;</span></div>
                <div class="stl_01" style="top:21.186em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:22.3115em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:23.4368em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:24.5623em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">6 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">output</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:25.6878em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:25.6878em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;">ꢀ stdout</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;"> { codec </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0002em;">=</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">&gt;</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> rubydebug</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> } &nbsp;</span></div>
                <div class="stl_01" style="top:26.8133em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">8 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:29.3886em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">7</span></div>
                <div class="stl_01" style="top:29.3886em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">.4.3</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">、启动测试 &nbsp;</span></div>
                <div class="stl_01" style="top:32.1906em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:33.3161em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:34.4416em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:35.5671em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:36.6925em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:37.818em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:38.9434em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:40.0688em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:41.1943em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:42.3198em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:43.4453em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:44.5708em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:45.6963em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:46.8218em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:47.9473em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:49.0727em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:50.1982em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:51.3236em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:32.1906em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">启动 &nbsp;</span></div>
                <div class="stl_01" style="top:33.3161em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0007em;">./bin/logstash </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0007em;">-f </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0007em;">./itcast-pipeline.conf &nbsp;</span></div>
                <div class="stl_01" style="top:35.5671em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">写日志到文件 &nbsp;</span></div>
                <div class="stl_01" style="top:36.6925em; left:6.8154em;"><span class="stl_21 stl_08 stl_09" style="word-spacing:-0.0005em;">echo </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0005em;">"2019-03-15 21:21:21|ERROR|</span><span class="stl_48 stl_08 stl_09" style="word-spacing:-0.0005em;">读取数据出错</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0005em;">|</span><span class="stl_48 stl_08 stl_09" style="word-spacing:-0.0005em;">参数：</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0005em;">id=1002" </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;">&gt;&gt; app.log &nbsp;</span></div>
                <div class="stl_01" style="top:38.9434em; left:6.8154em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">输出的结果 &nbsp;</span></div>
                <div class="stl_01" style="top:40.0688em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">{</span></div>
                <div class="stl_01" style="top:41.1943em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0002em;">"@timestamp" </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0002em;">=</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">&gt; </span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0002em;">2019</span><span class="stl_20 stl_08 stl_30" style="word-spacing:-0.0002em;">-03-15T08</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">:44:04.749Z, &nbsp;</span></div>
                <div class="stl_01" style="top:42.3198em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"path" </span><span class="stl_44 stl_08 stl_30" style="word-spacing:0em;">=</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">&gt; </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"/itcast/logstash/logs/app.log"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:43.4453em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">ꢀ ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"@version" </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0003em;">=</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">&gt; </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"1"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:44.5708em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"host" </span><span class="stl_44 stl_08 stl_30" style="word-spacing:0.0001em;">=</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">&gt; </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;">"node01"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:45.6963em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">ꢀ ꢀ ꢀ </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0002em;">"message" </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0002em;">=</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">&gt; [ &nbsp;</span></div>
                <div class="stl_01" style="top:42.3198em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:43.4453em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:44.5708em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:45.6963em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:46.8218em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:47.9473em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:49.0727em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:50.1982em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:51.3236em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:52.4491em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:46.8218em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ ꢀ ꢀ</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6026em;"> [0]</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;"> "2019-03-15</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0001em;"> 21:21:21"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:47.9473em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">ꢀ ꢀ ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;"> [1]</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0001em;"> "ERROR"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:49.0727em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;"> [2]</span><span class="stl_29 stl_08 stl_09" style="word-spacing:0.6026em;"> "</span><span class="stl_48 stl_08 stl_09" style="word-spacing:-0.0002em;">读取数据出错</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0002em;">"</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:50.1982em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;"> [3]</span><span class="stl_29 stl_08 stl_09" style="word-spacing:0.6025em;"> "</span><span class="stl_48 stl_08 stl_09" style="word-spacing:-0.0002em;">参数：</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0002em;">id=1002" &nbsp;</span></div>
                <div class="stl_01" style="top:51.3236em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ ] &nbsp;</span></div>
                <div class="stl_01" style="top:52.4491em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:55.0696em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">可以看到，数据已经被分割了。 &nbsp;</span></div>
                <div class="stl_01" style="top:57.0878em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">7</span></div>
                <div class="stl_01" style="top:57.0878em; left:4.5816em;"><span class="stl_40 stl_08 stl_49" style="font-weight:bold;">.4.5</span><span class="stl_41 stl_08 stl_49" style="font-weight:bold;">、输出到</span><span class="stl_40 stl_08 stl_49" style="font-weight:bold;">Elasticsearch &nbsp;</span></div>
                <div class="stl_01" style="top:59.8898em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:61.0151em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:62.1406em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:63.2661em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:64.3916em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:59.8898em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">input { &nbsp;</span></div>
                <div class="stl_01" style="top:61.0151em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ file { &nbsp;</span></div>
                <div class="stl_01" style="top:62.1406em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;"> path</span><span class="stl_44 stl_08 stl_09" style="word-spacing:0.6026em;"> =</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0013em;">&gt;</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0005em;"> "/itcast/logstash/logs/app.log" &nbsp;</span></div>
                <div class="stl_01" style="top:63.2661em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">#type =&gt; "system" &nbsp;</span></div>
                <div class="stl_01" style="top:64.3916em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;"> start_position</span><span class="stl_44 stl_08 stl_09" style="word-spacing:0.6026em;"> =</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.001em;">&gt;</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0005em;"> "beginning" &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_82.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_82.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.804em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:5.9295em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:7.055em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:8.1805em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:9.306em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:10.4315em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:11.557em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:4.804em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ } &nbsp;</span></div>
                <div class="stl_01" style="top:5.9295em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">}</span></div>
                <div class="stl_01" style="top:8.1805em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">filter { &nbsp;</span></div>
                <div class="stl_01" style="top:9.306em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:10.4315em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:11.557em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:12.6823em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:13.8078em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:14.9333em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:16.0588em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:17.1842em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:18.3097em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:19.4352em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:20.5607em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:21.6862em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:22.8117em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:23.937em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:25.0625em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:26.188em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:27.3135em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:9.306em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ mutate</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:10.4315em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">ꢀ ꢀ</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.6028em;"> split</span><span class="stl_44 stl_08 stl_31" style="word-spacing:0.6028em;"> =</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">&gt;</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;"> {</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0003em;">"message"</span><span class="stl_44 stl_08 stl_31" style="word-spacing:0.0003em;">=</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">&gt;</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0003em;">"|"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:11.557em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ } &nbsp;</span></div>
                <div class="stl_01" style="top:12.6823em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:13.8078em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:14.9333em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">output</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:16.0588em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:16.0588em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ elasticsearch</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:17.1842em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:17.1842em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ ꢀ ꢀ</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6026em;"> hosts</span><span class="stl_44 stl_08 stl_30" style="word-spacing:0.6026em;"> =</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0006em;">&gt;</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;"> [</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;"> "192.168.40.133:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">,</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;">"192.168.40.134:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">,</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;">"192.168.40.135:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:18.3097em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ } &nbsp;</span></div>
                <div class="stl_01" style="top:18.3097em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:19.4352em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:20.5607em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:21.6862em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:22.8117em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">启动 &nbsp;</span></div>
                <div class="stl_01" style="top:23.937em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">./bin/logstash</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0009em;"> -f</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;"> ./itcast-pipeline.conf &nbsp;</span></div>
                <div class="stl_01" style="top:25.0625em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:26.188em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">写入数据 &nbsp;</span></div>
                <div class="stl_01" style="top:27.3135em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">6 </span><span class="stl_21 stl_08 stl_09" style="word-spacing:0.7645em;">echo</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0012em;"> "2019-03-15</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0009em;"> 21:21:21|ERROR|</span><span class="stl_48 stl_08 stl_09" style="word-spacing:-0.0009em;">读取数据出错</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0009em;">|</span><span class="stl_48 stl_08 stl_09" style="word-spacing:-0.0009em;">参数：</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0009em;">id=1003" </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0009em;">&gt;&gt;</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> app.log &nbsp;</span></div>
                <div class="stl_01" style="top:29.934em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">测试： &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_85.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_85.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:31.549em; left:4.0017em;"><span class="stl_12 stl_08 stl_09" style="font-weight:bold;">8</span><span class="stl_07 stl_08 stl_09" style="font-weight:bold;">、综合练习 &nbsp;</span></div>
                <div class="stl_01" style="top:34.6235em; left:4.0017em;"><span class="stl_11 stl_08 stl_37" style="word-spacing:0.0007em;">下面我们将前面所学习到的</span><span class="stl_10 stl_08 stl_37" style="word-spacing:0.0007em;">Elasticsearch + Logstash + Beats + Kibana</span><span class="stl_11 stl_08 stl_37" style="word-spacing:0.0007em;">整合起来做一个综合性的练习，目的就是让 &nbsp;</span></div>
                <div class="stl_01" style="top:35.8739em; left:4.0017em;"><span class="stl_11 stl_08 stl_09" style="word-spacing:0em;">学生们能够更加深刻的理解</span><span class="stl_10 stl_08 stl_09" style="word-spacing:0em;">Elastic Stack</span><span class="stl_11 stl_08 stl_09" style="word-spacing:0em;">的使用。 &nbsp;</span></div>
                <div class="stl_01" style="top:37.9719em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">8</span></div>
                <div class="stl_01" style="top:37.9719em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.1</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、流程说明 &nbsp;</span></div>
                <div class="stl_01" style="top:53.9441em; left:5.8775em;"><span class="stl_11 stl_08 stl_09">应用</span><span class="stl_10 stl_08 stl_09">APP</span><span class="stl_11 stl_08 stl_09">生产日志，用来记录用户的操作 &nbsp;</span></div>
                <div class="stl_01" style="top:55.6322em; left:7.7533em;"><span class="stl_10 stl_08 stl_09">[</span></div>
                <div class="stl_01" style="top:55.6322em; left:8.0208em;"><span class="stl_10 stl_08 stl_35" style="word-spacing:0.0012em;">INFO] 2019-03-15 22:55:20 [cn.itcast.dashboard.Main] - DAU|5206|</span><span class="stl_11 stl_08 stl_35" style="word-spacing:0.0012em;">使用优惠券</span><span class="stl_10 stl_08 stl_35" style="word-spacing:0.0012em;">|2019-03-15 &nbsp;</span></div>
                <div class="stl_01" style="top:56.8827em; left:8.218em;"><span class="stl_10 stl_08 stl_09">3:37:20 &nbsp;</span></div>
                <div class="stl_01" style="top:58.1334em; left:8.0208em;"><span class="stl_10 stl_08 stl_42" style="word-spacing:0.0011em;">INFO] 2019-03-15 22:55:21 [cn.itcast.dashboard.Main] - DAU|3880|</span><span class="stl_11 stl_08 stl_42" style="word-spacing:0.0011em;">浏览页面</span><span class="stl_10 stl_08 stl_42" style="word-spacing:0.0011em;">|2019-03-15 07:25:09 &nbsp;</span></div>
                <div class="stl_01" style="top:56.8827em; left:7.7533em;"><span class="stl_10 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:58.1334em; left:7.7533em;"><span class="stl_10 stl_08 stl_09">[</span></div>
                <div class="stl_01" style="top:59.3839em; left:5.8775em;"><span class="stl_11 stl_08 stl_09">通过</span><span class="stl_10 stl_08 stl_09">Filebeat</span><span class="stl_11 stl_08 stl_09">读取日志文件中的内容，并且将内容发送给</span><span class="stl_10 stl_08 stl_09">Logstash</span><span class="stl_11 stl_08 stl_09">，原因是需要对内容做处理 &nbsp;</span></div>
                <div class="stl_01" style="top:61.0095em; left:5.8775em;"><span class="stl_10 stl_08 stl_45">Logstash</span><span class="stl_11 stl_08 stl_45">接收到内容后，进行处理，如分割操作，然后将内容发送到</span><span class="stl_10 stl_08 stl_45">Elasticsearch</span><span class="stl_11 stl_08 stl_45">中 &nbsp;</span></div>
                <div class="stl_01" style="top:62.6977em; left:5.8775em;"><span class="stl_10 stl_08 stl_15">Kibana</span><span class="stl_11 stl_08 stl_15">会读取</span><span class="stl_10 stl_08 stl_15">Elasticsearch</span><span class="stl_11 stl_08 stl_15">中的数据，并且在</span><span class="stl_10 stl_08 stl_15">Kibana</span><span class="stl_11 stl_08 stl_15">中进行设计</span><span class="stl_10 stl_08 stl_15">Dashboard</span><span class="stl_11 stl_08 stl_15">，最后进行展示 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_86.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_86.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.9234em; left:5.1897em;"><span class="stl_50 stl_08 stl_26" style="font-weight:bold;">说明：日志格式、图表、</span><span class="stl_51 stl_08 stl_26" style="font-weight:bold;">Dashboard</span><span class="stl_50 stl_08 stl_26" style="font-weight:bold;">都是自定义的。 &nbsp;</span></div>
                <div class="stl_01" style="top:7.0214em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">8</span></div>
                <div class="stl_01" style="top:7.0214em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.2</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">APP</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">介绍 &nbsp;</span></div>
                <div class="stl_01" style="top:9.4879em; left:4.0017em;"><span class="stl_10 stl_08 stl_09">APP</span><span class="stl_11 stl_08 stl_09">在生产环境应该是真实的系统，然而，我们现在仅仅的学习，为了简化操作，所以就做数据的模拟生成即可。 &nbsp;</span></div>
                <div class="stl_01" style="top:11.3637em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">业务代码如下： &nbsp;</span></div>
                <div class="stl_01" style="top:13.9953em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:15.1208em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:16.2463em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:17.3717em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:18.4972em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:19.6227em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:20.7482em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:21.8737em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:22.9992em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:13.9953em; left:6.8154em;"><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0004em;">package </span><span class="stl_43 stl_08 stl_30" style="word-spacing:-0.0004em;">cn</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0004em;">itcast</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0004em;">dashboard</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">; &nbsp;</span></div>
                <div class="stl_01" style="top:16.2463em; left:6.8154em;"><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0001em;">import </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">org</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">apache</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">commons</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">lang3</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">RandomUtils</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">; &nbsp;</span></div>
                <div class="stl_01" style="top:17.3717em; left:6.8154em;"><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0001em;">import </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">org</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">joda</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">time</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">DateTime</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">; &nbsp;</span></div>
                <div class="stl_01" style="top:18.4972em; left:6.8154em;"><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0001em;">import </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">org</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">slf4j</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">Logger</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">; &nbsp;</span></div>
                <div class="stl_01" style="top:19.6227em; left:6.8154em;"><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0001em;">import </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">org</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">slf4j</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">LoggerFactory</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">; &nbsp;</span></div>
                <div class="stl_01" style="top:20.7482em; left:6.8154em;"><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0002em;">import </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;">org</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;">springframework</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;">boot</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;">autoconfigure</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;">SpringBootApplication</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">; &nbsp;</span></div>
                <div class="stl_01" style="top:22.9992em; left:6.8154em;"><span class="stl_33 stl_08 stl_09">@SpringBootApplication &nbsp;</span></div>
                <div class="stl_01" style="top:24.1245em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:25.25em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:26.3755em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:27.501em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:28.6265em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:24.1245em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_34 stl_08 stl_09" style="word-spacing:0.7645em;">public</span><span class="stl_34 stl_08 stl_09" style="word-spacing:-0.0004em;"> class</span><span class="stl_43 stl_08 stl_09" style="word-spacing:-0.0014em;"> Main</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0014em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:25.25em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:26.3755em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:27.501em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:28.6265em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:26.3755em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">ꢀ ꢀ</span><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0003em;">private static final </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0003em;">Logger LOGGER </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0003em;">= </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0003em;">LoggerFactory</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0003em;">getLogger</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">(</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0003em;">Main</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">.</span><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0003em;">class</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">); &nbsp;</span></div>
                <div class="stl_01" style="top:28.6265em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0005em;">ꢀ ꢀ</span><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0005em;">public static final </span><span class="stl_53 stl_08 stl_30" style="word-spacing:-0.0005em;">String</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0005em;">[] </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0005em;">VISIT </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0005em;">= </span><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0005em;">new </span><span class="stl_53 stl_08 stl_30" style="word-spacing:-0.0005em;">String</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0005em;">[]{</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0005em;">"</span><span class="stl_48 stl_08 stl_30" style="word-spacing:-0.0005em;">浏览页面</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0005em;">"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0005em;">, </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0005em;">"</span><span class="stl_48 stl_08 stl_30" style="word-spacing:-0.0005em;">评论商品</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0005em;">"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0005em;">, </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0005em;">"</span><span class="stl_48 stl_08 stl_30" style="word-spacing:-0.0005em;">加入收藏</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0005em;">"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0005em;">, &nbsp;</span></div>
                <div class="stl_01" style="top:29.7519em; left:7.2562em;"><span class="stl_48 stl_08 stl_30" style="word-spacing:-0.0003em;">加入购物车</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">, </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"</span><span class="stl_48 stl_08 stl_30" style="word-spacing:-0.0003em;">提交订单</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">, </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"</span><span class="stl_48 stl_08 stl_30" style="word-spacing:-0.0003em;">使用优惠券</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">, </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"</span><span class="stl_48 stl_08 stl_30" style="word-spacing:-0.0003em;">领取优惠券</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">, </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"</span><span class="stl_48 stl_08 stl_30" style="word-spacing:-0.0003em;">搜索</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">, </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"</span><span class="stl_48 stl_08 stl_30" style="word-spacing:-0.0003em;">查看订单</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0003em;">"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">}; &nbsp;</span></div>
                <div class="stl_01" style="top:29.7519em; left:6.8154em;"><span class="stl_29 stl_08 stl_09">"</span></div>
                <div class="stl_01" style="top:30.8774em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:32.0029em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:33.1284em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:34.2539em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:35.3792em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:36.5047em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:37.6302em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:38.7557em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:39.8812em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:41.0067em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:42.1322em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:43.2576em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:44.3831em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:45.5086em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:46.6341em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:47.7594em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:48.8849em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:50.0104em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:51.1359em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:52.2614em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:53.3869em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:54.5124em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:55.6379em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:56.7633em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:30.8774em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:32.0029em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:33.1284em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:34.2539em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:35.3792em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:36.5047em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:37.6302em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:38.7557em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:39.8812em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:41.0067em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:42.1322em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:43.2576em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:44.3831em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:45.5086em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:46.6341em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:47.7594em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:48.8849em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:50.0104em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:51.1359em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:52.2614em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:53.3869em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:54.5124em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:32.0029em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">ꢀ ꢀ</span><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0004em;">public static </span><span class="stl_53 stl_08 stl_30" style="word-spacing:-0.0004em;">void </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0004em;">main</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">(</span><span class="stl_53 stl_08 stl_30" style="word-spacing:-0.0004em;">String</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">[] </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0004em;">args</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">) </span><span class="stl_34 stl_08 stl_30" style="word-spacing:-0.0004em;">throws </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0004em;">Exception </span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">{ &nbsp;</span></div>
                <div class="stl_01" style="top:33.1284em; left:7.2562em;"><span class="stl_19 stl_08 stl_37" style="word-spacing:0.0005em;">ꢀ ꢀ ꢀ ꢀ</span><span class="stl_34 stl_08 stl_37" style="word-spacing:0.0005em;">while</span><span class="stl_19 stl_08 stl_37" style="word-spacing:0.0005em;">(</span><span class="stl_27 stl_08 stl_37" style="word-spacing:0.0005em;">true</span><span class="stl_19 stl_08 stl_37" style="word-spacing:0.0005em;">){ &nbsp;</span></div>
                <div class="stl_01" style="top:34.2539em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_53 stl_08 stl_30" style="word-spacing:-0.0003em;">Long </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0003em;">sleep </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0003em;">= </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0003em;">RandomUtils</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0003em;">nextLong</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">(</span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0003em;">200</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">, </span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0003em;">1000 </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0003em;">* </span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0003em;">5</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0003em;">); &nbsp;</span></div>
                <div class="stl_01" style="top:35.3792em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_52 stl_08 stl_31" style="word-spacing:0.0003em;">Thread</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">.</span><span class="stl_52 stl_08 stl_31" style="word-spacing:0.0003em;">sleep</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">(</span><span class="stl_52 stl_08 stl_31" style="word-spacing:0.0003em;">sleep</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">); &nbsp;</span></div>
                <div class="stl_01" style="top:36.5047em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_53 stl_08 stl_30" style="word-spacing:-0.0002em;">Long </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;">maxUserId </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0002em;">= </span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0002em;">9999L</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">; &nbsp;</span></div>
                <div class="stl_01" style="top:37.6302em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_53 stl_08 stl_30" style="word-spacing:-0.0001em;">Long </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">userId </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0001em;">= </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">RandomUtils</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">nextLong</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">(</span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0001em;">1</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">, </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">maxUserId</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">); &nbsp;</span></div>
                <div class="stl_01" style="top:38.7557em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_53 stl_08 stl_30" style="word-spacing:-0.0001em;">String </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">visit </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0001em;">= </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">VISIT</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">[</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">RandomUtils</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">nextInt</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">(</span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0001em;">0</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">, </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">VISIT</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">length</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">)]; &nbsp;</span></div>
                <div class="stl_01" style="top:39.8812em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_52 stl_08 stl_09" style="word-spacing:-0.0003em;">DateTime now </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0003em;">= </span><span class="stl_34 stl_08 stl_09" style="word-spacing:-0.0003em;">new </span><span class="stl_52 stl_08 stl_09" style="word-spacing:-0.0003em;">DateTime</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">(); &nbsp;</span></div>
                <div class="stl_01" style="top:41.0067em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_53 stl_08 stl_30" style="word-spacing:-0.0002em;">int </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;">maxHour </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0002em;">= </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;">now</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;">getHourOfDay</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">(); &nbsp;</span></div>
                <div class="stl_01" style="top:42.1322em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_53 stl_08 stl_30" style="word-spacing:-0.0002em;">int </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;">maxMillis </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0002em;">= </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;">now</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;">getMinuteOfHour</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">(); &nbsp;</span></div>
                <div class="stl_01" style="top:43.2576em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_53 stl_08 stl_09" style="word-spacing:-0.0003em;">int </span><span class="stl_52 stl_08 stl_09" style="word-spacing:-0.0003em;">maxSeconds </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0003em;">= </span><span class="stl_52 stl_08 stl_09" style="word-spacing:-0.0003em;">now</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">.</span><span class="stl_52 stl_08 stl_09" style="word-spacing:-0.0003em;">getSecondOfMinute</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">(); &nbsp;</span></div>
                <div class="stl_01" style="top:44.3831em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_53 stl_08 stl_30" style="word-spacing:-0.0001em;">String </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">date </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0001em;">= </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">now</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">plusHours</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">(</span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0001em;">-</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">(</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">RandomUtils</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">nextInt</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">(</span><span class="stl_28 stl_08 stl_30" style="word-spacing:-0.0001em;">0</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">, </span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0001em;">maxHour</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">))) &nbsp;</span></div>
                <div class="stl_01" style="top:45.5086em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0003em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0003em;"> .</span><span class="stl_52 stl_08 stl_30" style="word-spacing:0.6028em;">plusMinutes</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6028em;">(</span><span class="stl_44 stl_08 stl_30" style="word-spacing:0.6028em;">-</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6028em;">(</span><span class="stl_52 stl_08 stl_30" style="word-spacing:0.6028em;">RandomUtils</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6028em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:0.6028em;">nextInt</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6028em;">(</span><span class="stl_28 stl_08 stl_30" style="word-spacing:0.6028em;">0</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6028em;">,</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;"> maxMillis</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">))) &nbsp;</span></div>
                <div class="stl_01" style="top:46.6341em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0003em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0003em;"> .</span><span class="stl_52 stl_08 stl_30" style="word-spacing:0.6028em;">plusSeconds</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6028em;">(</span><span class="stl_44 stl_08 stl_30" style="word-spacing:0.6028em;">-</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6028em;">(</span><span class="stl_52 stl_08 stl_30" style="word-spacing:0.6028em;">RandomUtils</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6028em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:0.6028em;">nextInt</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6028em;">(</span><span class="stl_28 stl_08 stl_30" style="word-spacing:0.6028em;">0</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6028em;">,</span><span class="stl_52 stl_08 stl_30" style="word-spacing:-0.0002em;"> maxSeconds</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">))) &nbsp;</span></div>
                <div class="stl_01" style="top:47.7594em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;"> .</span><span class="stl_52 stl_08 stl_30" style="word-spacing:0.6027em;">toString</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6027em;">(</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.6027em;">"yyyy-MM-dd</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;"> HH:mm:ss"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">); &nbsp;</span></div>
                <div class="stl_01" style="top:50.0104em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_53 stl_08 stl_09" style="word-spacing:-0.0004em;">String </span><span class="stl_52 stl_08 stl_09" style="word-spacing:-0.0004em;">result </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0004em;">= </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"DAU|" </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0004em;">+ </span><span class="stl_52 stl_08 stl_09" style="word-spacing:-0.0004em;">userId </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0004em;">+ </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"|" </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0004em;">+ </span><span class="stl_52 stl_08 stl_09" style="word-spacing:-0.0004em;">visit </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0004em;">+ </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0004em;">"|" </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0004em;">+ </span><span class="stl_52 stl_08 stl_09" style="word-spacing:-0.0004em;">date</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0004em;">; &nbsp;</span></div>
                <div class="stl_01" style="top:51.1359em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">ꢀ ꢀ ꢀ ꢀ ꢀ ꢀ</span><span class="stl_52 stl_08 stl_30" style="word-spacing:0.0002em;">LOGGER</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">.</span><span class="stl_52 stl_08 stl_30" style="word-spacing:0.0002em;">info</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">(</span><span class="stl_52 stl_08 stl_30" style="word-spacing:0.0002em;">result</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">); &nbsp;</span></div>
                <div class="stl_01" style="top:52.2614em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> } &nbsp;</span></div>
                <div class="stl_01" style="top:54.5124em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ } &nbsp;</span></div>
                <div class="stl_01" style="top:55.6379em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">7 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:56.7633em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:59.3839em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">运行结果： &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_87.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_87.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:5.3669em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:7.6178em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:9.8686em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:12.1196em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:14.3706em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:16.6216em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:18.8726em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:21.1234em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:23.3743em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:5.3669em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">[INFO] </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">2019</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">-03-15 </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">22</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">:54:42 [cn.itcast.dashboard.Main] </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">DAU|4645|</span><span class="stl_39 stl_08 stl_09" style="word-spacing:-0.0002em;">领取优惠券</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">|2019-03-15 &nbsp;</span></div>
                <div class="stl_01" style="top:6.4923em; left:6.7559em;"><span class="stl_28 stl_08 stl_30">7</span><span class="stl_19 stl_08 stl_30">:40:29 &nbsp;</span></div>
                <div class="stl_01" style="top:7.6178em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">[INFO] </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">2019</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">-03-15 </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">22</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">:54:44 [cn.itcast.dashboard.Main] </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">DAU|3482|</span><span class="stl_39 stl_08 stl_09" style="word-spacing:-0.0002em;">领取优惠券</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">|2019-03-15 &nbsp;</span></div>
                <div class="stl_01" style="top:8.7432em; left:6.7559em;"><span class="stl_28 stl_08 stl_30">8</span><span class="stl_19 stl_08 stl_30">:34:04 &nbsp;</span></div>
                <div class="stl_01" style="top:9.8686em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">[INFO] </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">2019</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">-03-15 </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">22</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">:54:48 [cn.itcast.dashboard.Main] </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">DAU|5607|</span><span class="stl_39 stl_08 stl_09" style="word-spacing:-0.0002em;">加入收藏</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">|2019-03-15 &nbsp;</span></div>
                <div class="stl_01" style="top:10.9941em; left:6.7559em;"><span class="stl_28 stl_08 stl_30">2</span><span class="stl_19 stl_08 stl_30">:44:09 &nbsp;</span></div>
                <div class="stl_01" style="top:12.1196em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">[INFO] </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">2019</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">-03-15 </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">22</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">:54:50 [cn.itcast.dashboard.Main] </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">DAU|9619|</span><span class="stl_39 stl_08 stl_09" style="word-spacing:-0.0002em;">加入收藏</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">|2019-03-15 &nbsp;</span></div>
                <div class="stl_01" style="top:13.2451em; left:6.7559em;"><span class="stl_28 stl_08 stl_30">1</span><span class="stl_19 stl_08 stl_30">:39:47 &nbsp;</span></div>
                <div class="stl_01" style="top:14.3706em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">[INFO] </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">2019</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">-03-15 </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">22</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">:54:53 [cn.itcast.dashboard.Main] </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">DAU|7666|</span><span class="stl_39 stl_08 stl_09" style="word-spacing:-0.0002em;">加入收藏</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">|2019-03-15 &nbsp;</span></div>
                <div class="stl_01" style="top:15.4961em; left:6.7559em;"><span class="stl_28 stl_08 stl_30">7</span><span class="stl_19 stl_08 stl_30">:47:18 &nbsp;</span></div>
                <div class="stl_01" style="top:16.6216em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">[INFO] </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">2019</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">-03-15 </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">22</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">:54:54 [cn.itcast.dashboard.Main] </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">DAU|4871|</span><span class="stl_39 stl_08 stl_09" style="word-spacing:-0.0002em;">提交订单</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">|2019-03-15 &nbsp;</span></div>
                <div class="stl_01" style="top:17.7471em; left:6.7559em;"><span class="stl_28 stl_08 stl_30">2</span><span class="stl_19 stl_08 stl_30">:36:27 &nbsp;</span></div>
                <div class="stl_01" style="top:18.8726em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">[INFO] </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">2019</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">-03-15 </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">22</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">:54:55 [cn.itcast.dashboard.Main] </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">DAU|7126|</span><span class="stl_39 stl_08 stl_09" style="word-spacing:-0.0002em;">加入收藏</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">|2019-03-15 &nbsp;</span></div>
                <div class="stl_01" style="top:19.9979em; left:6.7559em;"><span class="stl_28 stl_08 stl_30">6</span><span class="stl_19 stl_08 stl_30">:11:06 &nbsp;</span></div>
                <div class="stl_01" style="top:21.1234em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">[INFO] </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">2019</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">-03-15 </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">22</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">:55:00 [cn.itcast.dashboard.Main] </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">DAU|9606|</span><span class="stl_39 stl_08 stl_09" style="word-spacing:-0.0002em;">评论商品</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">|2019-03-15 &nbsp;</span></div>
                <div class="stl_01" style="top:22.2489em; left:6.7559em;"><span class="stl_28 stl_08 stl_30">2</span><span class="stl_19 stl_08 stl_30">:12:00 &nbsp;</span></div>
                <div class="stl_01" style="top:23.3743em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">[INFO] </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">2019</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">-03-15 </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0002em;">22</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">:55:02 [cn.itcast.dashboard.Main] </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0002em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">DAU|7698|</span><span class="stl_39 stl_08 stl_09" style="word-spacing:-0.0002em;">查看订单</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">|2019-03-15 &nbsp;</span></div>
                <div class="stl_01" style="top:24.4998em; left:6.7559em;"><span class="stl_28 stl_08 stl_30">8</span><span class="stl_19 stl_08 stl_30">:17:02 &nbsp;</span></div>
                <div class="stl_01" style="top:6.4923em; left:6.3152em;"><span class="stl_28 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:8.7432em; left:6.3152em;"><span class="stl_28 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:10.9941em; left:6.3152em;"><span class="stl_28 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:13.2451em; left:6.3152em;"><span class="stl_28 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:15.4961em; left:6.3152em;"><span class="stl_28 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:17.7471em; left:6.3152em;"><span class="stl_28 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:19.9979em; left:6.3152em;"><span class="stl_28 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:22.2489em; left:6.3152em;"><span class="stl_28 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:24.4998em; left:6.3152em;"><span class="stl_28 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:27.1204em; left:4.0017em;"><span class="stl_11 stl_08 stl_49">代码在资料中可以找到，</span><span class="stl_10 stl_08 stl_49">itcast-dashboard-generate.zip</span><span class="stl_11 stl_08 stl_49">。 &nbsp;</span></div>
                <div class="stl_01" style="top:28.9962em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">部署： &nbsp;</span></div>
                <div class="stl_01" style="top:31.6279em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:32.7533em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:33.8787em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:31.6279em; left:6.3152em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">打包成</span><span class="stl_22 stl_08 stl_09">jar</span><span class="stl_23 stl_08 stl_09">包，在</span><span class="stl_22 stl_08 stl_09">linux</span><span class="stl_23 stl_08 stl_09">上运行 &nbsp;</span></div>
                <div class="stl_01" style="top:32.7533em; left:6.3152em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0011em;">java </span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0011em;">-jar </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0011em;">itcast-dashboard-generate-1.0-SNAPSHOT.jar &nbsp;</span></div>
                <div class="stl_01" style="top:33.8787em; left:6.3152em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">运行之后，就可以将日志写入到</span><span class="stl_22 stl_08 stl_09">/itcast/logs/app.log</span><span class="stl_23 stl_08 stl_09">文件中 &nbsp;</span></div>
                <div class="stl_01" style="top:36.5339em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">8</span></div>
                <div class="stl_01" style="top:36.5339em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.3</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">Filebeat &nbsp;</span></div>
                <div class="stl_01" style="top:39.5687em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:40.6942em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:41.8197em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:42.9451em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:44.0706em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:45.1961em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:46.3214em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:47.4469em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:48.5724em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:39.5687em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">#vim itcast-dashboard.yml &nbsp;</span></div>
                <div class="stl_01" style="top:41.8197em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">filebeat.inputs: &nbsp;</span></div>
                <div class="stl_01" style="top:42.9451em; left:6.8154em;"><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0001em;">- </span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">type: log &nbsp;</span></div>
                <div class="stl_01" style="top:44.0706em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0013em;">enabled: </span><span class="stl_27 stl_08 stl_09" style="word-spacing:-0.0013em;">true &nbsp;</span></div>
                <div class="stl_01" style="top:45.1961em; left:7.6969em;"><span class="stl_19 stl_08 stl_09">paths: &nbsp;</span></div>
                <div class="stl_01" style="top:46.3214em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_20 stl_08 stl_30" style="word-spacing:0em;">- </span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">/itcast/logs/*.log &nbsp;</span></div>
                <div class="stl_01" style="top:47.4469em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">setup.template.settings: &nbsp;</span></div>
                <div class="stl_01" style="top:48.5724em; left:7.6969em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0009em;">index.number_of_shards: </span><span class="stl_28 stl_08 stl_09" style="word-spacing:-0.0009em;">3 &nbsp;</span></div>
                <div class="stl_01" style="top:49.6979em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:50.8234em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:51.9489em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:53.0744em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:54.1999em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:55.3254em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:49.6979em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">0 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">output.logstash: &nbsp;</span></div>
                <div class="stl_01" style="top:50.8234em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:51.9489em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:53.0744em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:50.8234em; left:7.6969em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">hosts: [</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0.0002em;">"192.168.40.133:5044"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0002em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:51.9489em; left:7.2562em;"><span class="stl_19 stl_08 stl_09">ꢀ</span></div>
                <div class="stl_01" style="top:53.0744em; left:7.2562em;"><span class="stl_19 stl_08 stl_09">ꢀ</span></div>
                <div class="stl_01" style="top:54.1999em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">4 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">启动 &nbsp;</span></div>
                <div class="stl_01" style="top:55.3254em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">./filebeat</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0013em;"> -e</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0007em;"> -c</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;"> itcast-dashboard.yml &nbsp;</span></div>
                <div class="stl_01" style="top:57.9805em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">8</span></div>
                <div class="stl_01" style="top:57.9805em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.4</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">Logstash &nbsp;</span></div>
                <div class="stl_01" style="top:61.0151em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:62.1406em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:63.2661em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:61.0151em; left:6.8154em;"><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;">#vim itcast-dashboard.conf &nbsp;</span></div>
                <div class="stl_01" style="top:63.2661em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">input { &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_88.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_88.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:4.804em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:5.9295em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:7.055em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:8.1805em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:9.306em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:10.4315em; left:5.3743em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:11.5568em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:12.6823em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:13.8078em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:14.9333em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:16.0588em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:17.1842em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:18.3097em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:19.4352em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:20.5607em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:21.6862em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">9</span></div>
                <div class="stl_01" style="top:22.8115em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:23.937em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:25.0625em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:26.188em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:27.3135em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:28.439em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:29.5644em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:30.6899em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:31.8154em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:4.804em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ beats { &nbsp;</span></div>
                <div class="stl_01" style="top:5.9295em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">ꢀ ꢀ port </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0003em;">=</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0003em;">&gt; </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0003em;">"5044" &nbsp;</span></div>
                <div class="stl_01" style="top:7.055em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ } &nbsp;</span></div>
                <div class="stl_01" style="top:8.1805em; left:6.8154em;"><span class="stl_19 stl_08 stl_09">}</span></div>
                <div class="stl_01" style="top:10.4315em; left:6.8154em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">filter { &nbsp;</span></div>
                <div class="stl_01" style="top:11.5568em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:12.6823em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:13.8078em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:14.9333em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:16.0588em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:17.1842em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:18.3097em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:19.4352em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:20.5607em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:21.6862em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:22.8115em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:23.937em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:25.0625em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:26.188em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:27.3135em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:28.439em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:29.5644em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:30.6899em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:31.8154em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:32.9409em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:34.0664em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:35.1917em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:36.3172em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:37.4427em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:38.5682em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:39.6937em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:40.8192em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:41.9447em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:43.0701em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:44.1956em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:45.3211em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:46.4466em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:47.5719em; left:4.9337em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:11.5568em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ mutate</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> {</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> ꢀ &nbsp;</span></div>
                <div class="stl_01" style="top:12.6823em; left:7.2562em;"><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">ꢀ ꢀ</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.6028em;"> split</span><span class="stl_44 stl_08 stl_31" style="word-spacing:0.6028em;"> =</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;">&gt;</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0001em;"> {</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0003em;">"message"</span><span class="stl_44 stl_08 stl_31" style="word-spacing:0.0003em;">=</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">&gt;</span><span class="stl_29 stl_08 stl_31" style="word-spacing:0.0003em;">"|"</span><span class="stl_19 stl_08 stl_31" style="word-spacing:0.0003em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:13.8078em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ } &nbsp;</span></div>
                <div class="stl_01" style="top:17.1842em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ mutate</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:18.3097em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;"> add_field</span><span class="stl_44 stl_08 stl_09" style="word-spacing:0.6026em;"> =</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0011em;">&gt;</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0011em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:19.4352em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">ꢀ ꢀ ꢀ ꢀ</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0002em;">"userId" </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0002em;">=</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0002em;">&gt; </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0002em;">"%{message[1]}" &nbsp;</span></div>
                <div class="stl_01" style="top:20.5607em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">ꢀ ꢀ ꢀ ꢀ</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0001em;">"visit" </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0001em;">=</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">&gt; </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0001em;">"%{message[2]}" &nbsp;</span></div>
                <div class="stl_01" style="top:21.6862em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">ꢀ ꢀ ꢀ ꢀ</span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0001em;">"date" </span><span class="stl_44 stl_08 stl_09" style="word-spacing:-0.0001em;">=</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0001em;">&gt; </span><span class="stl_29 stl_08 stl_09" style="word-spacing:-0.0001em;">"%{message[3]}" &nbsp;</span></div>
                <div class="stl_01" style="top:22.8115em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ ꢀ } &nbsp;</span></div>
                <div class="stl_01" style="top:23.937em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ } &nbsp;</span></div>
                <div class="stl_01" style="top:25.0625em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ mutate</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:26.188em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.0001em;">ꢀ ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6026em;"> convert</span><span class="stl_44 stl_08 stl_09" style="word-spacing:0.6026em;"> =</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0006em;">&gt;</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0006em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:27.3135em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">ꢀ ꢀ ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0002em;">"userId" </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0002em;">=</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0002em;">&gt; </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0002em;">"integer" &nbsp;</span></div>
                <div class="stl_01" style="top:28.439em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">ꢀ ꢀ ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"visit" </span><span class="stl_44 stl_08 stl_30" style="word-spacing:-0.0001em;">=</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0001em;">&gt; </span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0001em;">"string" &nbsp;</span></div>
                <div class="stl_01" style="top:29.5644em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">ꢀ ꢀ ꢀ ꢀ</span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"date" </span><span class="stl_44 stl_08 stl_30" style="word-spacing:0em;">=</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0em;">&gt; </span><span class="stl_29 stl_08 stl_30" style="word-spacing:0em;">"string" &nbsp;</span></div>
                <div class="stl_01" style="top:30.6899em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;">ꢀ ꢀ</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0em;"> } &nbsp;</span></div>
                <div class="stl_01" style="top:31.8154em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ } &nbsp;</span></div>
                <div class="stl_01" style="top:32.9409em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:34.0664em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:35.1917em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#output</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:36.3172em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> ꢀ</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.6025em;"> stdout</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> { codec =&gt;</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> rubydebug</span><span class="stl_22 stl_08 stl_09" style="word-spacing:0em;"> } &nbsp;</span></div>
                <div class="stl_01" style="top:37.4427em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">3 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#} &nbsp;</span></div>
                <div class="stl_01" style="top:38.5682em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:39.6937em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">5 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">output</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:40.8192em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">6</span></div>
                <div class="stl_01" style="top:40.8192em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ elasticsearch</span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;"> { &nbsp;</span></div>
                <div class="stl_01" style="top:41.9447em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">7</span></div>
                <div class="stl_01" style="top:41.9447em; left:7.2562em;"><span class="stl_19 stl_08 stl_30" style="word-spacing:0.0001em;">ꢀ ꢀ ꢀ</span><span class="stl_19 stl_08 stl_30" style="word-spacing:0.6026em;"> hosts</span><span class="stl_44 stl_08 stl_30" style="word-spacing:0.6026em;"> =</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0006em;">&gt;</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;"> [</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;"> "192.168.40.133:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">,</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;">"192.168.40.134:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">,</span><span class="stl_29 stl_08 stl_30" style="word-spacing:-0.0004em;">"192.168.40.135:9200"</span><span class="stl_19 stl_08 stl_30" style="word-spacing:-0.0004em;">] &nbsp;</span></div>
                <div class="stl_01" style="top:43.0701em; left:7.2562em;"><span class="stl_19 stl_08 stl_09" style="word-spacing:0.6025em;">ꢀ } &nbsp;</span></div>
                <div class="stl_01" style="top:43.0701em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">8</span></div>
                <div class="stl_01" style="top:44.1956em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">9 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">} &nbsp;</span></div>
                <div class="stl_01" style="top:45.3211em; left:5.3745em;"><span class="stl_18 stl_08 stl_09">0</span></div>
                <div class="stl_01" style="top:46.4466em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">1 </span><span class="stl_22 stl_08 stl_09" style="word-spacing:0.7645em;">#</span><span class="stl_23 stl_08 stl_09" style="word-spacing:0.7645em;">启动 &nbsp;</span></div>
                <div class="stl_01" style="top:47.5719em; left:5.3745em;"><span class="stl_18 stl_08 stl_09" style="word-spacing:0.7645em;">2 </span><span class="stl_19 stl_08 stl_09" style="word-spacing:0.7645em;">./bin/logstash</span><span class="stl_20 stl_08 stl_09" style="word-spacing:-0.0009em;"> -f</span><span class="stl_19 stl_08 stl_09" style="word-spacing:-0.0005em;"> itcast-dashboard.conf &nbsp;</span></div>
                <div class="stl_01" style="top:50.2271em; left:4.0017em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">8</span></div>
                <div class="stl_01" style="top:50.2271em; left:4.6976em;"><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">.5</span><span class="stl_14 stl_08 stl_09" style="font-weight:bold;">、</span><span class="stl_13 stl_08 stl_09" style="font-weight:bold;">Kibana &nbsp;</span></div>
                <div class="stl_01" style="top:52.6936em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">启动</span><span class="stl_10 stl_08 stl_09">Kibana</span><span class="stl_11 stl_08 stl_09">： &nbsp;</span></div>
                <div class="stl_01" style="top:55.3252em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">1</span></div>
                <div class="stl_01" style="top:56.4507em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">2</span></div>
                <div class="stl_01" style="top:57.5762em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">3</span></div>
                <div class="stl_01" style="top:58.7017em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">4</span></div>
                <div class="stl_01" style="top:59.8271em; left:4.8741em;"><span class="stl_18 stl_08 stl_09">5</span></div>
                <div class="stl_01" style="top:55.3252em; left:6.3152em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">启动 &nbsp;</span></div>
                <div class="stl_01" style="top:56.4507em; left:6.3152em;"><span class="stl_19 stl_08 stl_09">./bin/kibana &nbsp;</span></div>
                <div class="stl_01" style="top:58.7017em; left:6.3152em;"><span class="stl_22 stl_08 stl_09">#</span><span class="stl_23 stl_08 stl_09">通过浏览器进行访问 &nbsp;</span></div>
                <div class="stl_01" style="top:59.8271em; left:6.3152em;"><span class="stl_19 stl_08 stl_09">http://192.168.40.133:5601/app/kibana &nbsp;</span></div>
                <div class="stl_01" style="top:62.4477em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">添加</span><span class="stl_10 stl_08 stl_09">Logstash</span><span class="stl_11 stl_08 stl_09">索引到</span><span class="stl_10 stl_08 stl_09">Kibana</span><span class="stl_11 stl_08 stl_09">中： &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_91.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_91.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:27.1376em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">8</span></div>
                <div class="stl_01" style="top:27.1376em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">.5.1</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">、时间间隔的柱形图 &nbsp;</span></div>
                <div class="stl_01" style="top:51.5055em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">说明：</span><span class="stl_10 stl_08 stl_09">x</span><span class="stl_11 stl_08 stl_09">轴是时间，以天为单位，</span><span class="stl_10 stl_08 stl_09">y</span><span class="stl_11 stl_08 stl_09">轴是</span><span class="stl_10 stl_08 stl_09">count</span><span class="stl_11 stl_08 stl_09">数 &nbsp;</span></div>
                <div class="stl_01" style="top:53.3813em; left:4.0017em;"><span class="stl_11 stl_08 stl_26">保存：（</span><span class="stl_10 stl_08 stl_26">my-dashboard-</span><span class="stl_11 stl_08 stl_26">时间间隔的柱形图） &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_94.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_94.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:24.8866em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">8</span></div>
                <div class="stl_01" style="top:24.8866em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">.5.2</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">、各个操作的饼图分布 &nbsp;</span></div>
                <div class="stl_01" style="top:49.5671em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">统计各个操作的数量，形成饼图。 &nbsp;</span></div>
                <div class="stl_01" style="top:51.443em; left:4.0017em;"><span class="stl_11 stl_08 stl_26">保存：（</span><span class="stl_10 stl_08 stl_26">my-dashboard-</span><span class="stl_11 stl_08 stl_26">各个操作的饼图） &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_97.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_97.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:24.2615em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">8</span></div>
                <div class="stl_01" style="top:24.2615em; left:4.5816em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">.5.3</span><span class="stl_41 stl_08 stl_09" style="font-weight:bold;">、数据表格 &nbsp;</span></div>
                <div class="stl_01" style="top:45.9408em; left:4.0017em;"><span class="stl_11 stl_08 stl_09">在数据探索中进行保存，并且保存，将各个操作的数据以表格的形式展现出来。 &nbsp;</span></div>
                <div class="stl_01" style="top:47.8165em; left:4.0017em;"><span class="stl_11 stl_08 stl_32">保存：（</span><span class="stl_10 stl_08 stl_32">my-dashboard-</span><span class="stl_11 stl_08 stl_32">表格） &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
    <div class="stl_02">
        <div class="stl_03">
            <object data="030213212139_files/img_100.svg" type="image/svg+xml" class="stl_04" style="position:absolute; width:49.5833em; height:70.0833em;">
                <embed src="030213212139_files/img_100.svg" type="image/svg+xml" class="stl_04" />
            </object>
        </div>
        <div class="view">
            <div class="stl_05 stl_06">
                <div class="stl_01" style="top:28.3881em; left:4.0017em;"><span class="stl_40 stl_08 stl_09" style="font-weight:bold;">8</span></div>
                <div class="stl_01" style="top:28.3881em; left:4.5816em;"><span class="stl_40 stl_08 stl_54" style="font-weight:bold;">.5.4</span><span class="stl_41 stl_08 stl_54" style="font-weight:bold;">、制作</span><span class="stl_40 stl_08 stl_54" style="font-weight:bold;">Dashboard &nbsp;</span></div>
                <div class="stl_01" style="top:57.0079em; left:4.0017em;"><span class="stl_10 stl_08 stl_09">ꢀ</span></div>
                <div class="stl_01" style="top:67.063em; left:13.5417em;"><span class="stl_16 stl_17 stl_09">北京市昌平区建材城西路金燕龙办公楼一层 &nbsp;</span></div>
                <div class="stl_01" style="top:67.063em; left:29.2917em;"><span class="stl_16 stl_17 stl_09">电话：400-618-9090 &nbsp;</span></div>
            </div>
        </div>
    </div>
</body>
