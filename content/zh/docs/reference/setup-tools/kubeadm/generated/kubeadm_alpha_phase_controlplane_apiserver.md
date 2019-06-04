
生成 API 服务器的静态 Pod 清单
<!--
Generates the API server static Pod manifest
-->

<!--
### Synopsis
-->

### 概要

<!--
Generates the static Pod manifest file for the API server and saves it into /etc/kubernetes/manifests/kube-apiserver.yaml file. 
-->
为 API 服务器生成静态 Pod 清单文件，并将其保存到 /etc/kubernetes/manifests/kube-apiserver.yaml 文件中。

<!--
Alpha Disclaimer: this command is currently alpha.
-->
Alpha 免责声明：此命令目前属于 alpha。

```
kubeadm alpha phase controlplane apiserver [flags]
```

<!--
### Options
-->

### 选项

<table style="width: 100%; table-layout: fixed;">
  <colgroup>
    <col span="1" style="width: 10px;" />
    <col span="1" />
  </colgroup>
  <tbody>

    <tr>
      <td colspan="2">--apiserver-advertise-address string</td>
    </tr>
    <tr>
      <td></td><td style="line-height: 130%; word-wrap: break-word;">可用来访问 API 服务器的 IP 地址</td>
    </tr>
<!--
      <td></td><td style="line-height: 130%; word-wrap: break-word;">The IP address of the API server is accessible on</td>
-->

    <tr>
      <td colspan="2">--apiserver-bind-port int32&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;默认值： 6443</td>
    </tr>
<!--
      <td colspan="2">--apiserver-bind-port int32&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Default: 6443</td>
-->
    <tr>
      <td></td><td style="line-height: 130%; word-wrap: break-word;">可用来访问 API 服务器的端口号</td>
    </tr>
<!--
      <td></td><td style="line-height: 130%; word-wrap: break-word;">The port the API server is accessible on</td>
-->

    <tr>
      <td colspan="2">--apiserver-extra-args mapStringString</td>
    </tr>
    <tr>
      <td></td><td style="line-height: 130%; word-wrap: break-word;">一组以 &lt;flagname&gt;=&lt;value&gt; 的格式传递给 API 服务器或覆盖默认参数的附加的参数;</td>
    </tr>
<!--
     <td></td><td style="line-height: 130%; word-wrap: break-word;">A set of extra flags to pass to the API Server or override default ones in form of &lt;flagname&gt;=&lt;value&gt;</td>
-->

    <tr>
      <td colspan="2">--cert-dir string&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;默认值： "/etc/kubernetes/pki"</td>
    </tr>
<!--
      <td colspan="2">--cert-dir string&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Default: "/etc/kubernetes/pki"</td>
-->

    <tr>
      <td></td><td style="line-height: 130%; word-wrap: break-word;">存储证书的路径</td>
    </tr>
<!--
      <td></td><td style="line-height: 130%; word-wrap: break-word;">The path where certificates are stored</td>
-->

    <tr>
      <td colspan="2">--config string</td>
    </tr>
    <tr>
      <td></td><td style="line-height: 130%; word-wrap: break-word;">kubeadm 配置文件的路径 警告: 配置文件的使用是实验性的</td>
    </tr>
<!--
      <td></td><td style="line-height: 130%; word-wrap: break-word;">Path to kubeadm config file. WARNING: Usage of a configuration file is experimental</td>
-->

    <tr>
      <td colspan="2">--feature-gates string</td>
    </tr>
    <tr>
      <td></td><td style="line-height: 130%; word-wrap: break-word;">键值对集合，用来描述多种功能特性的特性开关；可选项有：<br/>Auditing=true|false (ALPHA - 默认=false)<br/>CoreDNS=true|false (默认=true)<br/>DynamicKubeletConfig=true|false (BETA - 默认=false)</td>
    </tr>
<!--
      <td></td><td style="line-height: 130%; word-wrap: break-word;">A set of key=value pairs that describe feature gates for various features. Options are:<br/>Auditing=true|false (ALPHA - default=false)<br/>CoreDNS=true|false (default=true)<br/>DynamicKubeletConfig=true|false (BETA - default=false)</td>
-->

    <tr>
      <td colspan="2">-h, --help</td>
    </tr>
    <tr>
      <td></td><td style="line-height: 130%; word-wrap: break-word;">apiserver 的帮助信息</td>
    </tr>
<!--
      <td></td><td style="line-height: 130%; word-wrap: break-word;">help for apiserver</td>
-->

    <tr>
      <td colspan="2">--kubernetes-version string&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;默认值： "stable-1"</td>
    </tr>
<!--
      <td colspan="2">--kubernetes-version string&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Default: "stable-1"</td>
-->
    <tr>
      <td></td><td style="line-height: 130%; word-wrap: break-word;">为控制平面选择一个特定的 Kubernetes 版本</td>
    </tr>
<!--
      <td></td><td style="line-height: 130%; word-wrap: break-word;">Choose a specific Kubernetes version for the control plane</td>
-->

    <tr>
      <td colspan="2">--service-cidr string&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;默认值： "10.96.0.0/12"</td>
    </tr>
<!--
      <td colspan="2">--service-cidr string&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Default: "10.96.0.0/12"</td>
-->

    <tr>
      <td></td><td style="line-height: 130%; word-wrap: break-word;">用于 Pod 网络的 IP 地址范围</td>
    </tr>
<!--
      <td></td><td style="line-height: 130%; word-wrap: break-word;">The range of IP address used for service VIPs</td>
-->

  </tbody>
</table>



<!--
### Options inherited from parent commands
-->

### 从父命令继承的选项

<table style="width: 100%; table-layout: fixed;">
  <colgroup>
    <col span="1" style="width: 10px;" />
    <col span="1" />
  </colgroup>
  <tbody>

    <tr>
      <td colspan="2">--rootfs string</td>
    </tr>
    <tr>
      <td></td><td style="line-height: 130%; word-wrap: break-word;">[实验] 到'真实'主机根文件系统的路径。</td>
    </tr>
<!--
     <td></td><td style="line-height: 130%; word-wrap: break-word;">[EXPERIMENTAL] The path to the 'real' host root filesystem.</td>
-->

  </tbody>
</table>


