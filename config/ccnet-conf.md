# ccnet.conf 配置

通过修改`ccnet/ccnet.conf`文件，可以对 Seafile
的网络选项进行设置，示例如下:

    [General]

    # 该设置不再使用
    USER_NAME=example

    # 请不要改变这个 ID.
    ID=eb812fd276432eff33bcdde7506f896eb4769da0

    # Seafile 服务器名称, 目前只出现在客户端日志中。
    NAME=example

    # Seahub(Seafile Web) 外部 URL，如果改值没有设对，会影响文件的上传下载。
    # 注意: 外部 URL 意味着"如果你使用 Nginx, 请使用 Nginx 对外的 URL"
    SERVICE_URL=http://www.example.com:8000


    [Network]

    # 该设置不再使用
    PORT=10001

    [Client]
    # 该设置不再使用
    PORT=13419

**注意**: 为使更改生效，请重启 Seafile.

    cd seafile-server
    ./seafile.sh restart
