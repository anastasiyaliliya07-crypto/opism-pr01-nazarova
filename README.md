# Практична робота № 1

**Дисципліна:** Основи побудови інформаційних систем та мереж

**Тема:** Спостереження за процесом звернення до вебресурсу. Побудова власної моделі рівнів взаємодії

| | |
|---|---|
| **Прізвище, ім'я** |Назарова Анастасія |
| **Група** |F5-2.02 |
| **Номер варіанта** |16 |
| **Домен варіанта** |netfilter.org |
| **Середовище виконання** | Windows |
| **Версія curl** | curl 8.13.0 (Windows) libcurl/8.13.0 Schannel zlib/1.3.1 WinIDN |
| **Дата виконання** |14.09.26 |

---

## Частина A. Збір експериментальних даних

### A.1. Запит із діагностичним виводом

**Команда:**

```
curl -v https://netfilter.org
```

**Вивід:**

```
* Host netfilter.org:443 was resolved.
* IPv6: (none)
* IPv4: 92.243.20.29
*   Trying 92.243.20.29:443...
* schannel: disabled automatic use of client certificate
* ALPN: curl offers http/1.1
* ALPN: server accepted http/1.1
* Connected to netfilter.org (92.243.20.29) port 443
* using HTTP/1.x
> GET / HTTP/1.1
> Host: netfilter.org
> User-Agent: curl/8.13.0
> Accept: */*
>
* Request completely sent off
< HTTP/1.1 200 OK
< Date: Sat, 12 Sep 2026 10:59:31 GMT
< Server: Apache
< Last-Modified: Tue, 01 Sep 2026 16:46:04 GMT
< ETag: "5e02-65a6ea78fedd5"
< Accept-Ranges: bytes
< Content-Length: 24066
< Vary: Accept-Encoding
< Content-Type: text/html
<
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" lang="en" xml:lang="en">
  <head xmlns="">
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" /><meta name="generator" content="Website XSL Stylesheet V2.6.0" /><link rel="next" href="about.html" title="About the netfilter/iptables project" /><link rel="bookmark" href="https://www.netfilter.org/" title="home" /><link rel="bookmark" href="https://www.netfilter.org/pub/" title="download" /><link rel="bookmark" href="https://git.netfilter.org/" title="git" /><link rel="bookmark" href="./mailinglists.html" title="lists" /><link rel="bookmark" href="https://bugzilla.netfilter.org/" title="bugzilla" /><link rel="bookmark" href="https://workshop.netfilter.org/" title="workshop" /><link rel="bookmark" href="https://patchwork.ozlabs.org/project/netfilter-devel/list/" title="patchwork" /><link rel="bookmark" href="https://wiki.nftables.org/" title="wiki" /><link rel="author" href="mailto:webmaster@netfilter.org" title="Contact webmaster" /><link rel="stylesheet" href="/style/netfilter.css" type="text/css" />
        <title xmlns="http://www.w3.org/1999/xhtml">netfilter/iptables project homepage
      -
    The netfilter.org project</title>

</head>
  <body>
    <div class="titlebar">
      <a href="index.html">
        <img class="titlebarleft" src="images/netfilter-logo3.png" alt="netfilter project logo" />
      </a>
    </div>
    <div class="linkbar"><a href="https://www.netfilter.org/">home</a> | <a href="https://www.netfilter.org/pub/">download</a> | <a href="https://git.netfilter.org/">git</a> | <a href="./mailinglists.html">lists</a> | <a href="https://bugzilla.netfilter.org/">bugzilla</a> | <a href="https://workshop.netfilter.org/">workshop</a> | <a href="https://patchwork.ozlabs.org/project/netfilter-devel/list/">patchwork</a> | <a href="https://wiki.nftables.org/">wiki</a></div>
    <div class="webpage">
      <a name="home" id="home"></a>
      <table class="layout" summary="Navigation">
        <tr>
          <td class="menu">
            <span class="toplevel">
              <a xmlns="" href="about.html" title="Who is behind the netfilter project">About</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/about.html#coreteam">Coreteam</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/about.html#history">History</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/about.html#license">License</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/about.html#thanks">Thanks</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/about.html#gpg">PGP key</a>
              <br />
            </span>
            <span class="toplevel">
              <a xmlns="" href="projects/index.html" title="Homepage of the netfilter.org projects">Projects</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/iptables/index.html" title="Homepage of the netfilter.org &quot;iptables&quot; project">iptables</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/nftables/index.html" title="Homepage of the netfilter.org &quot;nftables&quot; project">nftables</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/libnftnl/index.html" title="Homepage of the netfilter.org &quot;libnftnl&quot; project">libnftnl</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/libnfnetlink/index.html" title="Homepage of the netfilter.org &quot;libnfnetlink&quot; project">libnfnetlink</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/libnetfilter_acct/index.html" title="Homepage of the netfilter.org &quot;libnetfilter_acct&quot; project">libnetfilter_acct</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/libnetfilter_log/index.html" title="Homepage of the netfilter.org &quot;libnetfilter_log&quot; project">libnetfilter_log</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/libnetfilter_queue/index.html" title="Homepage of the netfilter.org &quot;libnetfilter_queue&quot; project">libnetfilter_queue</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/libnetfilter_conntrack/index.html" title="Homepage of the netfilter.org &quot;libnetfilter_conntrack&quot; project">libnetfilter_conntrack</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/libnetfilter_cttimeout/index.html" title="Homepage of the netfilter.org &quot;libnetfilter_cttimeout&quot; project">libnetfilter_cttimeout</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/libnetfilter_cthelper/index.html" title="Homepage of the netfilter.org &quot;libnetfilter_cthelper&quot; project">libnetfilter_cthelper</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/conntrack-tools/index.html" title="Homepage of the netfilter.org &quot;conntrack-tools&quot; project">conntrack-tools</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/libmnl/index.html" title="Homepage of the netfilter.org &quot;libmnl&quot; project">libmnl</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/nfacct/index.html" title="Homepage of the netfilter.org &quot;nfacct&quot; project">nfacct</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/ipset/index.html" title="Homepage of the netfilter.org &quot;ipset&quot; project">ipset</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/ulogd/index.html" title="Homepage of the netfilter.org &quot;ulogd&quot; project">ulogd</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="projects/xtables-addons/index.html" title="Homepage of the &quot;xtables-addons&quot; project">xtables-addons</a>
              <br />
            </span>
            <span class="toplevel">
              <a xmlns="" href="news.html" title="News of the netfilter project">News</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2026-09-01">nftables 1.1.7 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2026-08-31">libnftnl 1.3.2 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2026-03-04">iptables 1.8.13 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2026-02-19">iptables 1.8.12 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2026-02-04b">conntrack-tools 1.4.9 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2026-02-04">libnetfilter_conntrack 1.1.1 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2025-12-05">nftables 1.1.6 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2025-12-03">libnftnl 1.3.1 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2025-09-02">nftables 1.0.6.1 (stable) released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2025-08-27">nftables 1.1.5 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2025-08-06b">nftables 1.1.4 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2025-08-06">libnftnl 1.3.0 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2025-05-19">ulogd 2.0.9 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2025-04-22">nftables 1.1.3 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2025-04-14b">nftables 1.1.2 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2025-04-14">libnftnl 1.2.9 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2024-11-08">iptables 1.8.11 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2024-07-03b">nftables 1.1.1 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2024-10-03">libnftnl 1.2.8 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2024-09-25">libnetfilter_conntrack 1.1.0 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2024-07-16">nftables 1.1.0 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2024-07-15">libnftnl 1.2.7 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2023-11-17b">Arturo Borrero enters emeritus</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2023-11-17">Eric Leblond enters emeritus</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2023-10-19">nftables 1.0.9 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2023-10-10">iptables 1.8.10 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2023-09-29">conntrack-tools 1.4.8 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2023-07-14">nftables 1.0.8 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2023-07-11">libnftnl 1.2.6 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2023-03-13">nftables 1.0.7 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2023-03-09">libnftnl 1.2.5 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2023-01-12">iptables 1.8.9 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-12-21">nftables 1.0.6 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-11-10">libnftnl 1.2.4 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-11-02">ulogd 2.0.8 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-10-06">conntrack-tools 1.4.7 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-08-09b">nftables 1.0.5 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-08-09">libnftnl 1.2.3 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-06-07b">nftables 1.0.4 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-06-07">libnftnl 1.2.2 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-05-31">nftables 1.0.3 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-05-13">iptables 1.8.8 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-05-05b">libnetfilter_cttimeout 1.0.1 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-05-05">libnetfilter_cthelper 1.0.1 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-04-05b">libmnl 1.0.5 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-04-05">libnfnetlink 1.0.2 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-02-21">nftables 1.0.2 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-02-14">libnetfilter_conntrack 1.0.9 released</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/news.html#2022-01-24">settlement with Patrick McHardy</a>
              <br />
            </span>
            <span class="toplevel">
              <a xmlns="" href="documentation/index.html" title="Various documents published by the netfilter/iptables project">Documentation</a>
              <br />
            </span>
            <span class="toplevel">
              <a xmlns="" href="mailinglists.html">Mailing Lists</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/mailinglists.html#list-rules">List Rules</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/mailinglists.html#ml-announce">netfilter-announce list</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/mailinglists.html#ml-user">netfilter list</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/mailinglists.html#ml-devel">netfilter-devel list</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/mailinglists.html#ml-buglog">netfilter-buglog list</a>
              <br />
            </span>
            <span class="toplevel">
              <a xmlns="" href="contact.html" title="How to contact the netfilter project">Contact</a>
              <br />
            </span>
            <span class="toplevel">
              <a xmlns="" href="licensing.html" title="How to comply to the GPL license terms">Licensing</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/licensing.html#terms">GPL licensing terms</a>
              <br />
            </span>
            <span class="shrink1">
              <a xmlns="" href="/licensing.html#faq">GPL compliance FAQ</a>
              <br />
            </span>
            <span class="toplevel">
              <a xmlns="" href="support.html" title="How to help the netfilter project">Supporting netfilter</a>
              <br />
            </span>
            <br />
          </td>
          <td class="main">
            <h1 xmlns="">The netfilter.org project</h1>
            <div xmlns="" class="section"><div class="titlepage"><div><div><h2 class="title" style="clear: both"><a name="whatis" id="whatis"></a>What is the netfilter.org project?</h2></div></div></div>

<p>
The netfilter project is a community-driven collaborative
<a xmlns="http://www.w3.org/1999/xhtml" href="https://en.wikipedia.org/wiki/Free_and_open-source_software">FOSS</a>
project that provides packet filtering software for the <a xmlns="http://www.w3.org/1999/xhtml" href="http://www.kernel.org/">Linux</a> 2.4.x and later kernel series. The
netfilter project is commonly associated with <a href="projects/iptables/index.html" class="olink">iptables</a> and its successor <a href="projects/nftables/index.html" class="olink">nftables</a>.
</p>
<p>
The netfilter project enables packet filtering, network address [and port]
translation (NA[P]T), packet logging, userspace packet queueing and other
packet mangling.
</p>
<p>
The netfilter hooks are a framework inside the Linux kernel that allows kernel
modules to register callback functions at different locations of the Linux
network stack. The registered callback function is then called back for every
packet that traverses the respective hook within the Linux network stack.
</p>
<p>
<a href="projects/iptables/index.html" class="olink">iptables</a> is a generic firewalling
software that allows you to define rulesets.  Each rule within an IP table
consists of a number of classifiers (iptables matches) and one connected action
(iptables target).
</p>
<p>
<a href="projects/nftables/index.html" class="olink">nftables</a> is the successor of
<a href="projects/iptables/index.html" class="olink">iptables</a>, it allows for much more
flexible, scalable and performance packet classification. This is where all the
fancy new features are developed.
</p>
</div>
            <div xmlns="" class="section"><div class="titlepage"><div><div><h2 class="title" style="clear: both"><a name="features" id="features"></a>Main Features</h2></div></div></div>

<div class="itemizedlist"><ul class="itemizedlist" style="list-style-type: bullet; "><li class="listitem" style="list-style-type: disc">stateless packet filtering (IPv4 and IPv6)</li><li class="listitem" style="list-style-type: disc">stateful packet filtering (IPv4 and IPv6)</li><li class="listitem" style="list-style-type: disc">all kinds of network address and port translation, e.g. NAT/NAPT (IPv4 and IPv6)</li><li class="listitem" style="list-style-type: disc">flexible and extensible infrastructure</li><li class="listitem" style="list-style-type: disc">multiple layers of API's for 3rd party extensions</li></ul></div>
</div>
            <div xmlns="" class="section"><div class="titlepage"><div><div><h2 class="title" style="clear: both"><a name="whatcan" id="whatcan"></a>What can I do with netfilter?</h2></div></div></div>

<div class="itemizedlist"><ul class="itemizedlist" style="list-style-type: bullet; "><li class="listitem" style="list-style-type: disc">build internet firewalls based on stateless and stateful packet filtering</li><li class="listitem" style="list-style-type: disc">deploy highly available stateless and stateful firewall clusters</li><li class="listitem" style="list-style-type: disc">use NAT and masquerading for sharing internet access if you don't have enough public IP addresses</li><li class="listitem" style="list-style-type: disc">use NAT to implement transparent proxies</li><li class="listitem" style="list-style-type: disc">aid the tc and iproute2 systems used to build sophisticated QoS and policy routers</li><li class="listitem" style="list-style-type: disc">do further packet manipulation (mangling) like altering the TOS/DSCP/ECN bits of the IP header</li></ul></div>
</div>
            <div xmlns="" class="section"><div class="titlepage"><div><div><h2 class="title" style="clear: both"><a name="whynft" id="whynft"></a>What value does nftables provide?</h2></div></div></div>

<div class="itemizedlist"><ul class="itemizedlist" style="list-style-type: bullet; "><li class="listitem" style="list-style-type: disc">a single tool with consistent syntax as opposed to the fragmented {ip,ip6,eb,arp}tables and ipset</li><li class="listitem" style="list-style-type: disc">faster kernel-side transactional ruleset updates, no need for user-space locking</li><li class="listitem" style="list-style-type: disc">sets are more flexible and powerful than ipset, maps push the concept even further</li><li class="listitem" style="list-style-type: disc">full ruleset flexibility:
        <div class="itemizedlist"><ul class="itemizedlist" style="list-style-type: bullet; "><li class="listitem" style="list-style-type: disc">no pre-defined tables and chains</li><li class="listitem" style="list-style-type: disc">arbitrary number of user-defined tables to separate the ruleset into "namespaces"</li><li class="listitem" style="list-style-type: disc">base chain's hook and priority are configurable</li></ul></div>
        </li><li class="listitem" style="list-style-type: disc">more flexible rules: No mandatory parts (like counters), multiple actions allowed (e.g. log and drop)</li><li class="listitem" style="list-style-type: disc">ingress hook attaching a chain to an interface for early filtering right after TC</li><li class="listitem" style="list-style-type: disc">egress hook attaching a chain to an interface for transmit path filtering right before TC</li><li class="listitem" style="list-style-type: disc">flowtables provide a software fast path and hardware acceleration</li><li class="listitem" style="list-style-type: disc">some limited scripting ability embedded in the syntax (define variables, include other files), support for extensive scripting via JSON input and output</li></ul></div>
</div>
            <div xmlns="" class="section"><div class="titlepage"><div><div><h2 class="title" style="clear: both"><a name="licensing" id="licensing"></a>Licensing terms</h2></div></div></div>

<p>
netfilter.org develops software within the Linux kernel, which is released under the terms of the <a xmlns="http://www.w3.org/1999/xhtml" href="https://www.gnu.org/licenses/">GNU General Public License version 2 (GPL-2.0)</a> and compatible licenses. This project also provides userspace libraries and utilities that are released under the GPL-2.0, please consult licensing terms of each library and userspace tool specifically for details. For more information, <a href="licensing.html" class="olink">you can consult our licensing section</a>.
</p>
</div>
            <br />
          </td>
        </tr>
      </table>
    </div>
    <div>
      <span class="footerleft">
        <span xmlns="" class="copyright">Copyright © 1999-2025
                        The Netfilter webmasters
                . </span>
      </span>
      <span class="footerright">
        <a href="mailto:webmaster@netfilter.org">Contact webmaster</a>
      </span>
    </div>
  </body>
</html>
* Connection #0 to host netfilter.org left intact
```

---

### A.2. Запит без захисту з'єднання

**Команда:**

```
curl -v http://neverssl.com
```

**Вивід:**

```
* Host neverssl.com:80 was resolved.
* IPv6: (none)
* IPv4: 34.223.124.45
*   Trying 34.223.124.45:80...
* Connected to neverssl.com (34.223.124.45) port 80
* using HTTP/1.x
> GET / HTTP/1.1
> Host: neverssl.com
> User-Agent: curl/8.13.0
> Accept: */*
>
* Request completely sent off
< HTTP/1.1 200 OK
< Date: Sat, 12 Sep 2026 11:37:20 GMT
< Server: Apache/2.4.68 ()
< Upgrade: h2,h2c
< Connection: Upgrade
< Last-Modified: Wed, 29 Jun 2022 00:23:33 GMT
< ETag: "f79-5e28b29d38e93"
< Accept-Ranges: bytes
< Content-Length: 3961
< Vary: Accept-Encoding
< Content-Type: text/html; charset=UTF-8
<
<html>
        <head>
                <title>NeverSSL - Connecting ... </title>
                <style>
                body {
                        font-family: Montserrat, helvetica, arial, sans-serif;
                        font-size: 16x;
                        color: #444444;
                        margin: 0;
                }
                h2 {
                        font-weight: 700;
                        font-size: 1.6em;
                        margin-top: 30px;
                }
                p {
                        line-height: 1.6em;
                }
                .container {
                        max-width: 650px;
                        margin: 20px auto 20px auto;
                        padding-left: 15px;
                        padding-right: 15px
                }
                .header {
                        background-color: #42C0FD;
                        color: #FFFFFF;
                        padding: 10px 0 10px 0;
                        font-size: 2.2em;
                }
                .notice {
                        background-color: red;
                        color: white;
                        padding: 10px 0 10px 0;
                        font-size: 1.25em;
                        animation: flash 4s infinite;
                }
                @keyframes flash {
                0% {
                        background-color: red;
                }
                50% {
                        background-color: #AA0000;
                }
                0% {
                        background-color: red;
                }
                }
                <!-- CSS from Mark Webster https://gist.github.com/markcwebster/9bdf30655cdd5279bad13993ac87c85d -->
                </style>

                <script>
                        var adjectives = [ 'cool' , 'calm' , 'relaxed', 'soothing', 'serene', 'slow',
                                                        'beautiful', 'wonderful', 'wonderous', 'fun', 'good',
                                                        'glowing', 'inner', 'grand', 'majestic', 'astounding',
                                                        'fine', 'splendid', 'transcendent', 'sublime', 'whole',
                                                        'unique', 'old', 'young', 'fresh', 'clear', 'shiny',
                                                        'shining', 'lush', 'quiet', 'bright', 'silver' ];

                        var nouns =       [ 'day', 'dawn', 'peace', 'smile', 'love', 'zen', 'laugh',
                                                        'yawn', 'poem', 'song', 'joke', 'verse', 'kiss', 'sunrise',
                                                        'sunset', 'eclipse', 'moon', 'rainbow', 'rain', 'plan',
                                                        'play', 'chart', 'birds', 'stars', 'pathway', 'secret',
                                                        'treasure', 'melody', 'magic', 'spell', 'light', 'morning'];

                        var prefix =
                                        // Choose 3 zen adjectives
                                        adjectives.sort(function(){return 0.5-Math.random()}).slice(-3).join('')
                                        +
                                        // Coupled with a zen noun
                                        nouns.sort(function(){return 0.5-Math.random()}).slice(-1).join('');
                        window.location.href = 'http://' + prefix + '.neverssl.com/online';
                </script>
        </head>
        <body>
        <noscript>
                <div class="notice">
                        <div class="container">
                                ⚠️ JavaScript appears to be disabled. NeverSSL's cache-busting works better if you enable JavaScript for <code>neverssl.com</code>.
                        </div>
                </div>
        </noscript>
        <div class="header">
                <div class="container">
                <h1>NeverSSL</h1>
                </div>
        </div>
        <div class="content">
        <div class="container">

        <h1 id="status"></h1>
        <script>document.querySelector("#status").textContent = "Connecting ...";</script>
        <noscript>

                <h2>What?</h2>
                <p>This website is for when you try to open Facebook, Google, Amazon, etc
                on a wifi network, and nothing happens. Type "http://neverssl.com"
                into your browser's url bar, and you'll be able to log on.</p>

                <h2>How?</h2>
                <p>neverssl.com will never use SSL (also known as TLS). No
                encryption, no strong authentication, no <a
                href="https://en.wikipedia.org/wiki/HTTP_Strict_Transport_Security">HSTS</a>,
                no HTTP/2.0, just plain old unencrypted HTTP and forever stuck in the dark
                ages of internet security.</p>

                <h2>Why?</h2>
                <p>Normally, that's a bad idea. You should always use SSL and secure
                encryption when possible. In fact, it's such a bad idea that most websites
                are now using https by default.</p>

                <p>And that's great, but it also means that if you're relying on
                poorly-behaved wifi networks, it can be hard to get online.  Secure
                browsers and websites using https make it impossible for those wifi
                networks to send you to a login or payment page. Basically, those networks
                can't tap into your connection just like attackers can't. Modern browsers
                are so good that they can remember when a website supports encryption and
                even if you type in the website name, they'll use https.</p>

                <p>And if the network never redirects you to this page, well as you can
                see, you're not missing much.</p>

        <a href="https://twitter.com/neverssl">Follow @neverssl</a>

        </noscript>

        </div>
        </div>

        </body>
</html>
* Connection #0 to host neverssl.com left intact
```

---

### A.3. Запит до служби доменних імен

*Windows: `Resolve-DnsName ВАШ_ДОМЕН`*

**Команда (перше виконання):**

```
Resolve-DnsName netfilter.org
```

**Вивід:**

```
Name                                           Type   TTL   Section    IPAddress
----                                           ----   ---   -------    ---------
netfilter.org                                  AAAA   37953 Answer     2001:4b98:dc0:45:216:3eff:fe8c:1b05
netfilter.org                                  A      37084 Answer     92.243.20.29

```

**Команда (повторне виконання через 5–7 хвилин):**

```
Resolve-DnsName netfilter.org
```

**Вивід:**

```
Name                                           Type   TTL   Section    IPAddress
----                                           ----   ---   -------    ---------
netfilter.org                                  AAAA   37603 Answer     2001:4b98:dc0:45:216:3eff:fe8c:1b05
netfilter.org                                  A      36733 Answer     92.243.20.29

```

**Зафіксовані значення:**

| Параметр | Перше виконання | Повторне виконання |
|---|---|---|
| Час виконання (год:хв) |15:05 | 15:11|
| IP-адреса |92.243.20.29 | 92.243.20.29|
| Значення TTL |37084 |36733 |

---

### A.4. Контрольний ресурс

**Команда:**

```
curl -v https://google.com
```

**Вивід:**

```
* Host google.com:443 was resolved.
* IPv6: (none)
* IPv4: 142.250.120.139, 142.250.120.138, 142.250.120.102, 142.250.120.100, 142.250.120.101, 142.250.120.113
*   Trying 142.250.120.139:443...
* schannel: disabled automatic use of client certificate
* ALPN: curl offers http/1.1
* ALPN: server accepted http/1.1
* Connected to google.com (142.250.120.139) port 443
* using HTTP/1.x
> GET / HTTP/1.1
> Host: google.com
> User-Agent: curl/8.13.0
> Accept: */*
>
* Request completely sent off
< HTTP/1.1 301 Moved Permanently
< Location: https://www.google.com/
< Content-Type: text/html; charset=UTF-8
< Content-Security-Policy-Report-Only: object-src 'none';base-uri 'self';script-src 'nonce-hgiY6ak5NEysTKgkK-XW6A' 'strict-dynamic' 'report-sample' 'unsafe-eval' 'unsafe-inline' https: http:;report-uri https://csp.withgoogle.com/csp/gws/other-hp
< Date: Sat, 12 Sep 2026 12:26:40 GMT
< Expires: Mon, 12 Oct 2026 12:26:40 GMT
< Cache-Control: public, max-age=2592000
< Server: gws
< Content-Length: 220
< X-XSS-Protection: 0
< X-Frame-Options: SAMEORIGIN
< Alt-Svc: h3=":443"; ma=2592000,h3-29=":443"; ma=2592000
<
<HTML><HEAD><meta http-equiv="content-type" content="text/html;charset=utf-8">
<TITLE>301 Moved</TITLE></HEAD><BODY>
<H1>301 Moved</H1>
The document has moved
<A HREF="https://www.google.com/">here</A>.
</BODY></HTML>
* Connection #0 to host google.com left intact
```

---

### A.5. Ресурси з некоректною конфігурацією сертифіката

**Випадок 1**

```
curl -v https://expired.badssl.com
```

```
* Host expired.badssl.com:443 was resolved.
* IPv6: (none)
* IPv4: 104.154.89.105
*   Trying 104.154.89.105:443...
* schannel: disabled automatic use of client certificate
* ALPN: curl offers http/1.1
* schannel: next InitializeSecurityContext failed: SEC_E_CERT_EXPIRED (0x80090328) - The received certificate has expired.
* closing connection #0
curl: (35) schannel: next InitializeSecurityContext failed: SEC_E_CERT_EXPIRED (0x80090328) - The received certificate has expired.
```

**Випадок 2**

```
curl -v https://wrong.host.badssl.com
```

```
* Host wrong.host.badssl.com:443 was resolved.
* IPv6: (none)
* IPv4: 104.154.89.105
*   Trying 104.154.89.105:443...
* schannel: disabled automatic use of client certificate
* ALPN: curl offers http/1.1
* schannel: SNI or certificate check failed: SEC_E_WRONG_PRINCIPAL (0x80090322) - The target principal name is incorrect.
* closing connection #0
curl: (60) schannel: SNI or certificate check failed: SEC_E_WRONG_PRINCIPAL (0x80090322) - The target principal name is incorrect.
More details here: https://curl.se/docs/sslcerts.html

curl failed to verify the legitimacy of the server and therefore could not
establish a secure connection to it. To learn more about this situation and
how to fix it, please visit the webpage mentioned above.
```

**Випадок 3**

```
curl -v https://self-signed.badssl.com
```

```
* Host self-signed.badssl.com:443 was resolved.
* IPv6: (none)
* IPv4: 104.154.89.105
*   Trying 104.154.89.105:443...
* schannel: disabled automatic use of client certificate
* ALPN: curl offers http/1.1
* schannel: SEC_E_UNTRUSTED_ROOT (0x80090325) - The certificate chain was issued by an authority that is not trusted.
* closing connection #0
curl: (60) schannel: SEC_E_UNTRUSTED_ROOT (0x80090325) - The certificate chain was issued by an authority that is not trusted.
More details here: https://curl.se/docs/sslcerts.html

curl failed to verify the legitimacy of the server and therefore could not
establish a secure connection to it. To learn more about this situation and
how to fix it, please visit the webpage mentioned above.
```

---

## Частина B. Власна модель рівнів

**Кількість виділених груп:** 5

| № | Назва групи (власне формулювання) | Рядки виводу, віднесені до групи | Обґрунтування |
|---|---|---|---|
| 1 |Вебсторінка |HTML-код сторінок. `<html>`,<br>`<head>`,<br>`<body>`,<br>`<style>`,<br>`<title>`,<br>`<script>` | Це вміст (HTML/CSS/JS) HTTP-відповіді, який передається мережею для інтерпретації та відображення у браузері користувача. |
| 2 |Запит і відповідь | (запит): `> GET / HTTP/1.1`,<br>`> Host: netfilter.org`,<br> `> User-Agent: curl/8.13.0`,<br>`> Accept: */*`.  (відповідь): `< HTTP/1.1 200 OK`,<br>`< Date: Sat, 12 Sep 2026 10:59:31 GMT`,<br> `< Server: Apache`,<br>`< Last-Modified: Tue, 01 Sep 2026 16:46:04 GMT`,<br>`< ETag: "5e02-65a6ea78fedd5"`,<br>`< Accept-Ranges: bytes`,<br>`< Content-Length: 24066`,<br>`< Vary: Accept-Encoding`,<br>`< Content-Type: text/html`,<br>`< Server: Apache/2.4.68 ()`,<br>`< Upgrade: h2,h2c`,<br>`< Connection: Upgrade`,<br>`< Last-Modified: Wed, 29 Jun 2022 00:23:33 GMT`,<br>`< ETag: "f79-5e28b29d38e93"`,<br>`< Accept-Ranges: bytes`,<br>`< Content-Length: 3961`,<br>`< Vary: Accept-Encoding` |"Діалоги", якими комп'ютер і сервер обмінюються для організації зв'язку. Клієнт - запит, сервер - відповідь. |
| 3 |Захист і шифрування |`* schannel: disabled automatic use of client certificate`,<br>`* ALPN: curl offers http/1.1`,<br>`* schannel: next InitializeSecurityContext failed: SEC_E_CERT_EXPIRED ...`,<br>`* schannel: SNI or certificate check failed: SEC_E_WRONG_PRINCIPAL ...`,<br>`* schannel: SEC_E_UNTRUSTED_ROOT ...` |Це охорона. Йде перевірка процесу роботи захищеного TLS-з'єднання, узгодження протоколів шифрування та перевірка сертифікатів. На звичайному http:// її немає, а на https:// вона є, і вона перевіряє безпеку. Якщо сертифікат поганий - з'єднання розривається (closing connection). |
| 4 |DNS-адресація та розпізнавання імен |`netfilter.org AAAA 37953 Answer 2001:4b98:dc0:45:216:3eff:fe8c:1b05  netfilter.org A 37084 Answer 92.243.20.29`,<br>`netfilter.org AAAA 37603 Answer 2001:4b98:dc0:45:216:3eff:fe8c:1b05  netfilter.org A 36733 Answer 92.243.20.29` |Переклад зрозумілого імені сайту (наприклад, netfilter.org) у цифрову IP-адресу (наприклад, 92.243.20.29) за допомогою DNS-записів (A, AAAA) із зазначенням часу їх збереження в кеші (TTL). |
| 5 |Встановлення та завершення з'єднання |`* Host google.com:443 was resolved.`,<br>`* IPv6: (none)`,<br>`* IPv4: 142.250.120.139, 142.250.120.138, 142.250.120.102, 142.250.120.100, 142.250.120.101, 142.250.120.113`,<br>`* Trying 142.250.120.139:443...`,<br>`* Connected to google.com (142.250.120.139) port 443`,<br>`* Trying 104.154.89.105:443...`,<br>`* closing connection #0` |Факт того, що ПК проклав канал до конкретного сервера в Інтернеті за його IP-адресою і портом. |

*Групи впорядковано від найближчої до користувача (№ 1) до найближчої до апаратного забезпечення.*

**Рядки, які не вдалося віднести до жодної групи:**

| Рядок виводу | Причина утруднення |
|---|---|
|`* Request completely sent off` |Програма curl каже нам про те, що запит повністю відправлено на сервер (що буфер вихідних даних порожній). Це є просто повідомлення про внутрішній стан програми, а не про надісланий мережевий пакет чи HTTP-заголовок. |
|`* Connection #0 to host google.com left intact` |Повідомлення від curl, що вона не закрила підключення одразу, а тримає його готовим на випадок наступного запиту. |
|`* More details here: https://curl.se/docs/sslcerts.html` |Локальний текст, згенерований програмою curl для користувача при помилці сертифіката (із сервера вона не приходила).|

---

## Контрольні питання

**1. Скільки рядків діагностичного виводу передує отриманню даних сторінки (завдання A.1)?**

> До першої відповіді сервера 15 рядків. Рядки 1–9 (* ...) - процес встановлення з'єднання. Рядки 10–13 (> ...) - HTTP-запит клієнта. Рядок 14 (>) - порожній рядок-розділювач. Рядок 15 (* Request completely sent off) - діагностичне повідомлення curl (писала про нього раніше). А починаючи з 16-го рядка (`< HTTP/1.1 200 OK`), починається прийом даних відповіді від сервера.

**2. Які рядки наявні у виводі A.1 і відсутні у виводі A.2? Чим це зумовлено?**

> У виводі A.1 наявні рядки `* schannel: disabled automatic use of client certificate`,<br>`* ALPN: curl offers http/1.1`,<br>`* ALPN: server accepted http/1.1`, які відсутні в A.2. Це тому, що сайт netfilter.org використовує шифроване з'єднання HTTPS, а neverssl.com працює через незахищений протокол HTTP без шифрування.

**3. Звідки у виводі з'явилося значення `443`, якщо його не було вказано в адресі?**

> Значення `443` з'явилося тому, що порт `443` є стандартним портом за замовчуванням для протоколу HTTPS. Коли в адресі порт не вказується явно, curl автоматично підставляє стандартний порт для встановлення захищеного з'єднання.

**4. Як змінилося значення TTL між двома запитами (A.3)? Що означає це число?**

> Значення TTL між двома запитами зменшилося на 351 секунду (з `37953` до `37603` для `IPv6` та з `37084` до `36733` для `IPv4`). Число TTL (Time to Live) означає час у секундах, протягом якого DNS-сервер зберігає знайдену IP-адресу у своєму кеші. Зменшення цього числа показує зворотний відлік часу, що минув між моїми першим і другим запитами до того, як дані в кеші застаріють і оновляться.

**5. Чим відрізняються між собою три причини помилок із завдання A.5? Сформулювати кожну однією фразою.**

| Випадок | Причина недовіри |
|---|---|
| `expired` |Прострочений сертифікат |
| `wrong.host` |Сертифікат від іншого сайту |
| `self-signed` |Ненадійний видавець |

**6. Три рядки з власних виводів, про які не йшлося на лекції 1:**

| № | Рядки виводу | Джерело (номер завдання) |
|---|---|---|
| 1 |`* schannel: disabled automatic use of client certificate`<br>`* ALPN: curl offers http/1.1`<br>`* ALPN: server accepted http/1.1`  | А1, А4, А5 |
| 2 |`< ETag: "5e02-65a6ea78fedd5"`/`< ETag: "f79-5e28b29d38e93"`  |А1/А2 |
| 3 |`< X-XSS-Protection: 0`<br>`< X-Frame-Options: SAMEORIGIN`<br>`< Alt-Svc: h3=":443"; ma=2592000,h3-29=":443"; ma=2592000` |А4 |

*Пояснення до цих рядків не потрібне.*

---

## Висновки

*150–300 слів. Спиратися на власні спостереження, а не на матеріал лекції.*

**D.1. Що виявилося неочевидним або несподіваним**

*Назвати конкретно, з посиланням на рядок виводу.*

> Під час виконання практичної роботи цікаво було побачити реальну роботу таймера TTL у команді `Resolve-DnsName`. Між моїми двома запитами минуло біля 6 хвилин, і значення TTL зменшилося на 351 секунду (з `37953` до `37603` для `IPv6` та з `37084` до `36733` для `IPv4`). Це наочно показало, як DNS-сервер відраховує час до видалення IP-адреси зі свого кешу.  Також я побачила наскільки суттєво відрізняється службовий вивід curl для звичайного HTTP та захищеного HTTPS. У випадку з `netfilter.org` з'явилися додаткові рядки налаштування шифрування (`* schannel: disabled automatic use of client certificate`<br>`* ALPN: curl offers http/1.1`<br>`* ALPN: server accepted http/1.1`), а також стандартний порт `443`. Натомість для `neverssl.com` curl підключився напряму через порт `80` без жодних перевірок безпеки.  Я побачила як чітко curl розрізняє причини помилок SSL-сертифікатів і блокує з'єднання ще до отримання даних сторінки. У завданнях A.5 кожна помилка мала свій конкретний код і текстове пояснення: від застарілого терміну дії (`SEC_E_CERT_EXPIRED`) до невідповідності імені домену (`SEC_E_WRONG_PRINCIPAL`). Виявилося цікавим, що навіть якщо сервер технічно працює та віддає IP-адресу (наприклад, `104.154.89.105`), браузер чи curl миттєво розривають зв'язок (рядок `closing connection #0`), якщо сертифікат не є повністю довіреним.

**D.2. Чому саме така кількість груп у частині B**

*На якій підставі ухвалено рішення. Що змусило б його змінити.*

> Я виділила 5 груп, оскільки вони описують чітку послідовність кроків: спочатку йде пошук IP-адреси (DNS), далі встановлення зв'язку, потім перевірка безпеки (SSL), після цього HTTP-діалог запиту/відповіді і, нарешті, сам HTML-код сторінки.

**D.3. Питання, яке залишилося без відповіді**

> Як саме curl обирає, через яку адресу підключатися — `IPv4` чи `IPv6`, якщо сайт (як-от `netfilter.org`) повертає у відповіді `DNS` обидва варіанти одночасно?

---

## Використання штучного інтелекту

*Розділ обов'язковий. Заповнюється незалежно від того, чи використовувався ШІ. Детальні вимоги — у документі «Політика використання технологій штучного інтелекту».*

**Факт використання:** використано

**Установлений рівень для цієї роботи:** Р3 — ШІ як співвиконавець

**Фактичний рівень використання:** Р3 — ШІ як співвиконавець

### Використані системи

| Система | Версія або модель | Період використання |
|---|---|---|
|Gemini |Gemini 3.6 Flash |12.09.26-14.09.26 |

### Промпти

*Наводити дослівно, у тому вигляді, у якому запит було надано системі. Переказ не приймається.*

| № | Розділ роботи | Текст промпта |
|---|---|---|
| 1 |Частина В |Перевір плс, чи все норм? І чи впорядковані вони від найближчої до користувача до найближчої до апаратного забезпечення так, як треба?Власна модель рівнів:1. Назва: Сторінка, яку бачить користувач    Рядки виводу: HTML-код сторінок.<html>, <head>, <body>, <style>, <noscript>, <title>..    Обгрунтування: Це вміст (HTML/CSS/JS) HTTP-відповіді, який передається мережею для інтерпретації та відображення у браузері користувача.2. Назва: Запит і відповідь     Рядки виводу:  (відправка):> GET / HTTP/1.1> Host: netfilter.org / > Host: neverssl.com / > Host: google.com> User-Agent: curl/8.13.0> Accept: */*(відповідь):< HTTP/1.1 200 OK< Date: Sat, 12 Sep 2026 10:59:31 GMT< Server: Apache< Last-Modified: Tue, 01 Sep 2026 16:46:04 GMT< ETag: "5e02-65a6ea78fedd5"< Accept-Ranges: bytes< Content-Length: 24066< Vary: Accept-Encoding< Content-Type: text/html< Server: Apache/2.4.68 ()< Upgrade: h2,h2c< Connection: Upgrade< Last-Modified: Wed, 29 Jun 2022 00:23:33 GMT< ETag: "f79-5e28b29d38e93"< Accept-Ranges: bytes< Content-Length: 3961< Vary: Accept-Encoding    Обгрунтування: "діалоги", якими комп'ютер ісервер обмінюються для організації зв'язку. Клієн - запит, сервер - відповідь.3. Назва: Захист і шифрування    Рядки виводу: * schannel: disabled automatic use of client certificate* ALPN: curl offers http/1.1* schannel: next InitializeSecurityContext failed: SEC_E_CERT_EXPIRED ...(помилка: прострочений сертифікат)* schannel: SNI or certificate check failed: SEC_E_WRONG_PRINCIPAL ...(помилка: сертифікат від іншого сайту)* schannel: SEC_E_UNTRUSTED_ROOT ...(помилка: ненадійний видавець)    Обгрунтування: Це охорона. Йде перевірка процесу роботи захищеного TLS-з'єднання, узгодження протоколів шифрування та перевірка сертифікатів. На звичайному http:// її немає, а на https:// вона є, і вона перевіряє безпеку. Якщо сертифікат поганий - з'єднання розривається (closing connection).4. Назва: DNS-адресації та розпізнавання імен    Рядки виводу: netfilter.org AAAA 37953 Answer 2001:4b98:dc0:45:216:3eff:fe8c:1b05netfilter.org A 37084 Answer 92.243.20.29netfilter.org AAAA 37603 Answer 2001:4b98:dc0:45:216:3eff:fe8c:1b05netfilter.org A 36733 Answer 92.243.20.29  Обгрунтування: Переклад зрозумілого імені сайту (наприклад, netfiler.org) у цифровий IP-адрес (наприклад, 92.243.20.29) за допомогою DNS-записів (A, AAAA) із зазначенням часу їх збереження в кеші (TTL).5. Назва: Встановлення та завершення з'єднання  Рядки виводу: * Host google.com:443 was resolved.* IPv6: (none)* IPv4: 142.250.120.139, 142.250.120.138, 142.250.120.102, 142.250.120.100, 142.250.120.101, 142.250.120.113* Trying 142.250.120.139:443...* Connected to google.com (142.250.120.139) port 443* Trying 104.154.89.105:443...* closing connection #0   Обгрунтування: Факт того, що ПК проклав канал до конкретного сервера в Інтернеті за його IP-адресою і портом.    (вставила йому текст який накидувала в нотатках)|
| 2 |Частина В |Окей, дякую. Можеш виписати рядки виводу що не вдалося віднести до жодної групи, з моїх результатів. І чому  (надала йому свої виводи)|
| 3 |Контрольні питання |на основі моїх виводів, дай відповіді на питання, простими і зрозумілими словами  (прикріпила pdf з питаннями)|
| 4 |Висновки |сформуй гарний висновок плс|

### Дії з отриманим результатом

| № промпта | Що перевірено | Що змінено | Що відхилено і чому |
|---|---|---|---|
| 1 |Невеликі виправлення одруків у тексті |Виправила помилки у тексті |Вирішила змінити назву моєї 1ї групи з "Сторінка, яку бачить користувач" на "Вебсторінка", бо другий варіант коротше і простіше |
| 2 |Рядки виводу. Я їх залишила, оскільки згодна з ними |Обгрунтування. Я переписала так, як мені зрозуміло |-|
| 3 |Було перевірено на правдивість і точність за моїми виводами  |Усі відповіді були змінені і відкориговані мною |відповідь на перше питання повністю відхилена, бо була неправильною |
| 4 |Було порівняння відповіді з моєю думкою |Відповіді на D1 та D2 |-|

### Підтвердження

Підтверджую, що всі наведені в цьому звіті виводи команд отримано мною особисто внаслідок фактичного виконання відповідних дій, а відомості цього розділу є повними та достовірними.

> Виводи `curl`, `dig` та інші артефакти не можуть бути згенеровані. Це стосується будь-якого рівня використання ШІ.

---

