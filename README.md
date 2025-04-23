# **BlueTeam-Tools**

<p align="center">
<img src="https://user-images.githubusercontent.com/100603074/210680535-40d8c113-2336-4417-bdb4-4825a7477164.png" height="300">
</p>

Kho lưu trữ Github này chứa bộ sưu tập **65+** **công cụ** và **tài nguyên** có thể hữu ích cho các **hoạt động blue teaming**.

Một số **công cụ** có thể được thiết kế riêng cho **blue teaming**, trong khi những **công cụ** khác có tính chất tổng quát hơn và có thể được điều chỉnh để sử dụng trong bối cảnh **blue teaming**.

> 🔗 Nếu bạn là **Red Teamer**, hãy xem xét [**RedTeam-Tools**](https://github.com/A-poc/RedTeam-Tools)

> **Cảnh báo**
>
> *Các tài liệu trong kho lưu trữ này chỉ dành cho mục đích thông tin và giáo dục. Chúng không nhằm mục đích sử dụng trong bất kỳ hoạt động bất hợp pháp nào.*

> **Ghi chú**
>
> *Ẩn các tiêu đề của **Danh sách công cụ** bằng mũi tên.*
>
> *Nhấn 🔙 để quay lại danh sách.*

# **Danh sách công cụ**

<details open>
<summary><b>Mẹo Blue Team</b> 4 mẹo</summary>
    <ul>
        <ul>
            <li><b><a href="#payload-extraction-with-process-hacker">Trích xuất **payload** với **Process Hacker**</a></b><i> @embee_research</i></li>
            <li><b><a href="#prevent-script-execution-via-double-click">Ngăn chặn Thực thi Script thông qua Nhấp đúp</a></b><i> Thay đổi GPO Ứng dụng Mặc định</i></li>
            <li><b><a href="#detect-cryptojacking-malware-with-proxy-logs">Phát hiện **Malware Cryptojacking** với Nhật ký Proxy</a></b><i> Dave Mckay</i></li>
            <li><b><a href="#remove-null-bytes-in-cyberchef-malware-analysis">Xóa byte null trong phân tích **malware** với **CyberChef**</a></b><i> @Securityinbits</i></li>
        </ul>
    </ul>
</details>

<details open>
<summary><b>Khám phá và Ánh xạ Mạng</b> 6 công cụ</summary>
    <ul>
        <ul>
            <li><b><a href="#nmap">Nmap</a></b><i> Máy quét mạng</i></li>
            <li><b><a href="#nuclei">Nuclei</a></b><i> Máy quét lỗ hổng</i></li>
            <li><b><a href="#masscan">Masscan</a></b><i> Máy quét mạng nhanh</i></li>
            <li><b><a href="#angry-ip-scanner">Angry IP Scanner</a></b><i> Máy quét **IP/port**</i></li>
            <li><b><a href="#zmap">ZMap</a></b><i> Máy quét mạng lớn</i></li>
            <li><b><a href="#shodan">Shodan</a></b><i> Công cụ tìm kiếm tài sản hướng Internet</i></li>
        </ul>
    </ul>
</details>

<details open>
<summary><b>Quản lý Lỗ hổng</b> 4 công cụ</summary>
    <ul>
        <ul>
            <li><b><a href="#openvas">OpenVAS</a></b><i> Máy quét lỗ hổng nguồn mở</i></li>
            <li><b><a href="#nessus-essentials">Nessus Essentials</a></b><i> Máy quét lỗ hổng</i></li>
            <li><b><a href="#nexpose">Nexpose</a></b><i> Công cụ quản lý lỗ hổng</i></li>
            <li><b><a href="#hackerone">HackerOne</a></b><i> Nền tảng quản lý **Bug Bounty**</i></li>
        </ul>
    </ul>
</details>

<details open>
<summary><b>Giám sát An ninh</b> 10 công cụ</summary>
    <ul>
        <ul>
            <li><b><a href="#sysmon">Sysmon</a></b><i> **System Monitor** cho **Windows**</i></li>
            <li><b><a href="#kibana">Kibana</a></b><i> Trực quan hóa và khám phá dữ liệu</i></li>
            <li><b><a href="#logstash">Logstash</a></b><i> Thu thập và xử lý dữ liệu</i></li>
            <li><b><a href="#parsedmarc">parsedmarc</a></b><i> Trực quan hóa dữ liệu **DMARC Email**</i></li>
            <li><b><a href="#phishing-catcher">Phishing Catcher</a></b><i> Công cụ bắt **phishing** sử dụng **Certstream**</i></li>
            <li><b><a href="#maltrail">maltrail</a></b><i> Hệ thống phát hiện lưu lượng độc hại</i></li>
            <li><b><a href="#autorunstowineventlog">AutorunsToWinEventLog</a></b><i> Công cụ phân tích sự kiện Autoruns của **Windows**</i></li>
            <li><b><a href="#procfilter">procfilter</a></b><i> **Framework** chặn tiến trình tích hợp **YARA**</i></li>
            <li><b><a href="#velociraptor">velociraptor</a></b><i> Công cụ hiển thị và thu thập dữ liệu điểm cuối</i></li>
            <li><b><a href="#sysmonsearch">SysmonSearch</a></b><i> Trực quan hóa nhật ký sự kiện **Sysmon**</i></li>
        </ul>
    </ul>
</details>

<details open>
<summary><b>Công cụ và Kỹ thuật Đe dọa</b> 11 công cụ</summary>
    <ul>
        <ul>
            <li><b><a href="#lolbas-projectgithubio">lolbas-project.github.io</a></b><i> **Binary** Windows "**Living Off The Land**"</i></li>
            <li><b><a href="#gtfobinsgithubio">gtfobins.github.io</a></b><i> **Binary** Linux "**Living Off The Land**"</i></li>
            <li><b><a href="#filesecio">filesec.io</a></b><i> Phần mở rộng file của kẻ tấn công</i></li>
            <li><b><a href="#kql-search">KQL Search</a></b><i> Công cụ tổng hợp truy vấn **KQL**</i></li>
            <li><b><a href="#unprotect-project">Unprotect Project</a></b><i> Cơ sở kiến thức kỹ thuật né tránh **malware**</i></li>
            <li><b><a href="#chainsaw">chainsaw</a></b><i> Công cụ tìm kiếm Hiện vật Pháp y Windows nhanh</i></li>
            <li><b><a href="#freq">freq</a></b><i> Phát hiện **malware** bằng thuật toán tạo domain (**DGA**)</i></li>
            <li><b><a href="#yargen">yarGen</a></b><i> Công cụ tạo luật **YARA**</i></li>
            <li><b><a href="#emailanalyzer">EmailAnalyzer</a></b><i> Công cụ phân tích email đáng ngờ</i></li>
            <li><b><a href="#vcg">VCG</a></b><i> Công cụ quét bảo mật mã nguồn</i></li>
            <li><b><a href="#cyberchef">CyberChef</a></b><i> Nền tảng thao tác dữ liệu trực tuyến của GCHQ</i></li>
        </ul>
    </ul>
</details>

<details open>
<summary><b>Tình báo Đe dọa</b> 4 công cụ</summary>
    <ul>
        <ul>
            <li><b><a href="#maltego">Maltego</a></b><i> Nền tảng Tình báo Đe dọa</i></li>
            <li><b><a href="#misp">MISP</a></b><i> Nền tảng chia sẻ thông tin **Malware**</i></li>
            <li><b><a href="#threatconnect">ThreatConnect</a></b><i> Tổng hợp dữ liệu đe dọa</i></li>
            <li><b><a href="#adversary-emulation-library">Adversary Emulation Library</a></b><i> Thư viện kế hoạch mô phỏng kẻ thù nguồn mở</i></li>
        </ul>
    </ul>
</details>

<details open>
<summary><b>Lập kế hoạch Ứng phó Sự cố</b> 5 công cụ</summary>
    <ul>
        <ul>
            <li><b><a href="#nist">NIST</a></b><i> **Cybersecurity Framework**</i></li>
            <li><b><a href="#incident-response-plan">Kế hoạch Ứng phó Sự cố</a></b><i> **Framework** ứng phó sự cố</i></li>
            <li><b><a href="#ransomware-response-plan">Kế hoạch Ứng phó Ransomware</a></b><i> **Framework** ứng phó **ransomware**</i></li>
            <li><b><a href="#incident-response-reference-guide">Hướng dẫn Tham khảo Ứng phó Sự cố</a></b><i> Tài liệu hướng dẫn chuẩn bị sự cố</i></li>
            <li><b><a href="#awesome-incident-response">Awesome Incident Response</a></b><i> Danh sách các công cụ ứng phó sự cố</i></li>
        </ul>
    </ul>
</details>

<details open>
<summary><b>Phát hiện và Phân tích Malware</b> 11 công cụ</summary>
    <ul>
        <ul>
            <li><b><a href="#virustotal">VirusTotal</a></b><i> Nền tảng chia sẻ **IOC** độc hại</i></li>
            <li><b><a href="#ida">IDA</a></b><i> Trình dịch ngược và gỡ lỗi **Malware**</i></li>
            <li><b><a href="#ghidra">Ghidra</a></b><i> Công cụ dịch ngược phần mềm độc hại</i></li>
            <li><b><a href="#decode-vbe">decode-vbe</a></b><i> Công cụ giải mã script **VBE** được mã hóa</i></li>
            <li><b><a href="#pafish">pafish</a></b><i> Công cụ phát hiện **sandbox máy ảo**</i></li>
            <li><b><a href="#lookyloo">lookyloo</a></b><i> Ánh xạ domain **phishing**</i></li>
            <li><b><a href="#yara">YARA</a></b><i> Nhận dạng **Malware** thông qua khớp mẫu</i></li>
            <li><b><a href="#cuckoo-sandbox">Cuckoo Sandbox</a></b><i> **Sandbox** phân tích **Malware**</i></li>
            <li><b><a href="#radare2">Radare2</a></b><i> **Framework** dịch ngược</i></li>
            <li><b><a href="#dnspy">dnSpy</a></b><i> Công cụ gỡ lỗi và chỉnh sửa **assembly .NET**</i></li>
            <li><b><a href="#malware-traffic-analysisnet">malware-traffic-analysis.net</a></b><i> Mẫu **Malware** và packet capture</i></li>
        </ul>
    </ul>
</details>

<details open>
<summary><b>Phục hồi Dữ liệu</b> 3 công cụ</summary>
    <ul>
        <ul>
            <li><b><a href="#recuva">Recuva</a></b><i> Phục hồi tệp</i></li>
            <li><b><a href="#extundelete">Extundelete</a></b><i> Phục hồi phân vùng Ext3 hoặc Ext4</i></li>
            <li><b><a href="#testdisk">TestDisk</a></b><i> Phục hồi dữ liệu</i></li>
        </ul>
    </ul>
</details>

<details open>
<summary><b>Pháp y Kỹ thuật số</b> 3 công cụ</summary>
    <ul>
        <ul>
            <li><b><a href="#sans-sift">SANS SIFT</a></b><i> Bộ công cụ pháp y</i></li>
            <li><b><a href="#the-sleuth-kit">The Sleuth Kit</a></b><i> Công cụ phân tích ảnh đĩa</i></li>
            <li><b><a href="#autopsy">Autopsy</a></b><i> Nền tảng pháp y kỹ thuật số</i></li>
        </ul>
    </ul>
</details>

<details open>
<summary><b>Đào tạo Nhận thức An ninh</b> 4 công cụ</summary>
    <ul>
        <ul>
            <li><b><a href="#tryhackme">TryHackMe</a></b><i> Nền tảng thử thách an ninh mạng</i></li>
            <li><b><a href="#hackthebox">HackTheBox</a></b><i> Nền tảng thử thách an ninh mạng</i></li>
            <li><b><a href="#cyberdefenders">CyberDefenders</a></b><i> Nền tảng thử thách an ninh mạng cho **Blue Team**</i></li>
            <li><b><a href="#phishme">PhishMe</a></b><i> Đào tạo về **Phishing**</i></li>
        </ul>
    </ul>
</details>

<details open>
<summary><b>Giao tiếp và Cộng tác</b> 2 công cụ</summary>
    <ul>
        <ul>
            <li><b><a href="#twitter">Twitter</a></b><i> Các tài khoản An ninh mạng</i></li>
            <li><b><a href="#facebook-theatexchange">Facebook TheatExchange</a></b><i> Nền tảng chia sẻ chỉ báo độc hại</i></li>
        </ul>
    </ul>
</details>

**Mẹo Blue Team**
====================

*Học hỏi từ các **Blue Teamer** với bộ sưu tập Mẹo **Blue Teaming**. Những mẹo này bao gồm nhiều chiến thuật, **công cụ** và phương pháp luận để cải thiện khả năng **blue teaming** của bạn.*

### [🔙](#tool-list)Trích xuất **payload** với **Process Hacker**

![image](https://user-images.githubusercontent.com/100603074/217382117-acb26f85-d352-43b3-8818-6c5a0d90f350.png)

**Mô tả:**
*'Mẹo Phân tích **Malware** - Sử dụng **Process Hacker** để theo dõi các **assembly .NET** đáng ngờ trong các tiến trình mới được tạo ra. Kết hợp với **DnSpy**, có thể định vị và trích xuất các **payload** độc hại mà không cần phải giải mã thủ công.'*

**Đóng góp:** [@embee_research](https://twitter.com/embee_research)

**Liên kết:** [Twitter](https://twitter.com/embee_research/status/1614871485931458560)

### [🔙](#tool-list)Ngăn chặn Thực thi Script thông qua Nhấp đúp

![image](https://user-images.githubusercontent.com/100603074/218200763-53f9fc80-59e1-468a-93e2-69b84d1c7196.png)

**Mô tả:**
*Trên **Windows**, phổ biến khi thấy các tác nhân đe dọa đạt được thực thi ban đầu thông qua các tệp script độc hại giả mạo tệp **Microsoft Office**. Một cách hay để ngăn chặn chuỗi tấn công này là thay đổi ứng dụng mặc định liên kết với các tệp này (**HTA, JS, VBA, VBS**) thành `notepad.exe`. Bây giờ khi một người dùng bị lừa thành công nhấp vào tệp **HTA** trên đĩa, tệp sẽ mở script trong notepad và mã độc sẽ không được thực thi.*

**Đóng góp:** [bluesoul](https://bluesoul.me/)

**Liên kết:** [Blog](https://bluesoul.me/2016/05/12/use-gpo-to-change-the-default-behavior-of-potentially-malicious-file-extensions/)

### [🔙](#tool-list)Phát hiện **Malware Cryptojacking** với Nhật ký Proxy

**Mô tả:** ***Malware cryptojacking** ngày càng trở nên tinh vi hơn, với phần mềm đào tiền ảo sử dụng kỹ thuật **DLL sideloading** để ẩn mình trên máy và giảm tải **CPU** để nằm dưới ngưỡng phát hiện. Một điểm chung mà chúng đều có là phải tạo kết nối đến các mining pool, đây là nơi chúng ta có thể tìm thấy chúng. Hãy giám sát nhật ký **proxy** và **DNS** của bạn để tìm các kết nối chứa các chuỗi mining pool phổ biến (ví dụ: `*xmr.*` HOẶC `*pool.com` HOẶC `*pool.org` HOẶC `pool.*`).*

**Đóng góp:** [Dave Mckay](https://www.howtogeek.com/author/davidmckay/)

**Liên kết:** [Blog](https://www.howtogeek.com/devops/how-to-detect-and-defeat-cryptominers-in-your-network/)

### [🔙](#tool-list)Xóa byte null trong phân tích **malware** với **CyberChef**

![image](https://user-images.githubusercontent.com/100603074/223865015-00128d71-0093-4422-b271-e26dac723013.png)

**Mô tả:** *'Sau khi giải mã **base64** cho chuỗi **Unicode** trong quá trình phân tích **malware**, bạn có thể gặp phải các byte null. Giữ mã nguồn của bạn dễ đọc bằng cách sử dụng thao tác "Remove null bytes" trong **CyberChef**.'*

**Đóng góp:** [Ayush Anand](https://twitter.com/Securityinbits)

**Liên kết:** [Twitter](https://twitter.com/securityinbits/status/1628364983661694976)

**Khám phá và Ánh xạ Mạng**
====================

*Các công cụ để quét và ánh xạ mạng, khám phá thiết bị và dịch vụ, và nhận dạng các lỗ hổng tiềm ẩn.*

### [🔙](#tool-list)[**Nmap**](https://nmap.org)

**Nmap** (viết tắt của Network Mapper) là một **công cụ** quét mạng miễn phí và mã nguồn mở được sử dụng để khám phá các host và dịch vụ trên mạng máy tính, và thăm dò thông tin về các đặc điểm của chúng.

Nó có thể được sử dụng để xác định cổng nào trên mạng đang mở và dịch vụ nào đang chạy trên các cổng đó. Bao gồm khả năng nhận dạng các lỗ hổng bảo mật trên mạng.

**Cài đặt:**

You can download the latest release from [tại đây](https://nmap.org/download).
**Lưu ý:** **Nmap** là công cụ rất phổ biến và có trình cài đặt cho hầu hết các hệ điều hành.

**Cách sử dụng:**

```bash
# Quét một IP đơn
nmap 192.168.1.1

# Quét một dải địa chỉ
nmap 192.168.1.1-254

# Quét mục tiêu từ một tệp
nmap -iL targets.txt

# Quét cổng 21
nmap 192.168.1.1 -p 21

# Bật phát hiện HĐH, phát hiện phiên bản dịch vụ, quét script và traceroute
nmap 192.168.1.1 -A
```
**Lưu ý:** Đây là các ví dụ cơ bản về cách sử dụng `nmap` cho các tác vụ quét mạng. Các kết quả quét có thể được Blue Team sử dụng để kiểm tra các dịch vụ không mong muốn đang chạy, các cổng mở lộ ra ngoài không cần thiết, và thông tin phiên bản dịch vụ có thể chỉ ra các lỗ hổng đã biết.

Nice usage [cheat sheet](https://www.stationx.net/nmap-cheat-sheet/).

![image](https://user-images.githubusercontent.com/100603074/210288428-01875d96-72e6-4857-b18d-4e10d80863ad.png)

*Image used from https://kirelos.com/nmap-version-scan-determining-the-version-and-available-services/*

### [🔙](#tool-list)[**Nuclei**](https://nuclei.projectdiscovery.io/nuclei/get-started/)

A specialized tool designed to automate the process of detecting vulnerabilities in web applications, networks, and infrastructure.

**Nuclei** uses pre-defined templates to probe a target and identify potential vulnerabilities. It can be used to test a single host or a range of hosts, and can be configured to run a variety of tests to check for different types of vulnerabilities.

**Install:**

```bash
git clone https://github.com/projectdiscovery/nuclei.git; \
cd nuclei/v2/cmd/nuclei; \
go build; \
mv nuclei /usr/local/bin/; \
nuclei -version;
```
**Lưu ý:** Hướng dẫn cài đặt **Nuclei** bằng cách clone mã nguồn Golang, build và di chuyển file thực thi vào thư mục bin của hệ thống.

**Cách sử dụng:**

```bash
# Tất cả các template được thực thi từ đường dẫn cài đặt template mặc định.
nuclei -u https://example.com

# Thư mục template tùy chỉnh hoặc nhiều thư mục template
nuclei -u https://example.com -t cves/ -t exposures/

# Templates có thể được thực thi trên danh sách URL
nuclei -list http_urls.txt

# Loại trừ một template đơn lẻ
nuclei -list urls.txt -t cves/ -exclude-templates cves/2020/CVE-2020-XXXX.yaml
```
**Lưu ý:** Sử dụng **Nuclei** từ góc độ Blue Team rất quan trọng để tự kiểm tra hạ tầng của mình. Bạn có thể chạy các template công khai hoặc tự tạo/chỉnh sửa để tìm các lỗ hổng mà attacker có thể khai thác. Tích hợp vào quy trình kiểm tra định kỳ giúp đảm bảo an toàn liên tục.

Full usage information can be found [tại đây](https://nuclei.projectdiscovery.io/nuclei/get-started/#running-nuclei).

![image](https://user-images.githubusercontent.com/100603074/210288448-c2d9da7d-e68f-4d06-9066-b702ce4b5cb3.png)

*Image used from https://www.appsecsanta.com/nuclei*

### [🔙](#tool-list)[**Masscan**]()

A port scanner that is similar to **nmap**, but is much faster and can scan a large number of ports in a short amount of time.

**Masscan** uses a novel technique called "**SYN scan**" to scan networks, which allows it to scan a large number of ports very quickly.

**Install (Apt):**

```bash
sudo apt install masscan
```
**Lưu ý:** Cài đặt tiêu chuẩn trên các hệ thống Linux dựa trên Debian/Ubuntu.

**Install (Git):**

```bash
sudo apt-get install clang git gcc make libpcap-dev
git clone https://github.com/robertdavidgraham/masscan
cd masscan
make
```
**Lưu ý:** Biên dịch Masscan từ mã nguồn bằng Git và Make. Cần các thư viện phát triển (`libpcap-dev`).

**Cách sử dụng:**

```bash
# Quét các cổng 22, 80, 445 (-p22,80,445) trên subnet 192.168.1.0/24
masscan -p22,80,445 192.168.1.0/24

# Quét subnet lớp B cho các cổng 22 đến 25
masscan 10.11.0.0/16 -p22-25

# Quét subnet lớp B cho top 100 cổng với tốc độ 100.000 gói tin mỗi giây
masscan 10.11.0.0/16 ‐‐top-ports 100 ––rate 100000

# Quét subnet lớp B, nhưng bỏ qua các dải địa chỉ trong exclude.txt
masscan 10.11.0.0/16 ‐‐top-ports 100 ‐‐excludefile exclude.txt
```
**Lưu ý:** Masscan cực nhanh, có thể quét toàn bộ Internet trong thời gian ngắn. Blue Team có thể dùng nó để quét các dải IP lớn của tổ chức mình hoặc các mục tiêu bên ngoài liên quan, phát hiện nhanh các cổng đang mở mà các công cụ chậm hơn có thể bỏ sót hoặc mất quá nhiều thời gian. Cẩn trọng khi sử dụng `--rate` quá cao vì có thể gây ảnh hưởng đến mạng.

![image](https://user-images.githubusercontent.com/100603074/210288465-fa4d7b45-d7ff-4c5e-82a6-e0d480b387c7.png)

*Image used from https://kalilinuxtutorials.com/masscan/*

### [🔙](#tool-list)[**Angry IP Scanner**](https://angryip.org/)

A free and open-source tool for scanning IP addresses and ports.

It's a cross-platform tool, designed to be fast and easy to use, and can scan an entire network or a range of IP addresses to find live hosts.

**Angry IP Scanner** can also detect the hostname and MAC address of a device, and can be used to perform basic **ping sweeps** and port scans.

**Install:**

You can download the latest release from [tại đây](https://angryip.org/download/).
**Lưu ý:** Có phiên bản cài đặt cho Windows, macOS và Linux. Đây là công cụ quét IP/Port cơ bản, dễ sử dụng.

**Cách sử dụng:**

**Angry IP Scanner** can be used via the GUI.
**Lưu ý:** Chủ yếu sử dụng qua giao diện đồ họa.

Full usage information and documentation can be found [tại đây](https://angryip.org/documentation/).

![image](https://user-images.githubusercontent.com/100603074/210288485-711924ca-504e-4655-9e91-a0ecf32b2e63.png)

*Image used from https://angryip.org/screenshots/*

### [🔙](#tool-list)[**ZMap**](https://github.com/zmap/zmap)

**ZMap** is a network scanner designed to perform comprehensive scans of the IPv4 address space or large portions of it.

On a typical desktop computer with a gigabit Ethernet connection, **ZMap** is capable scanning the entire public IPv4 address space in under 45 minutes.
**Lưu ý:** Tương tự Masscan về tốc độ và khả năng quét phạm vi rộng, thường được dùng để khảo sát các dịch vụ cụ thể trên các dải IP công cộng hoặc mạng nội bộ lớn.

**Install:**

You can download the latest release from [tại đây](https://github.com/zmap/zmap/releases).

**Usage:**

```bash
# Quét chỉ 10.0.0.0/8 và 192.168.0.0/16 trên TCP/80
zmap -p 80 10.0.0.0/8 192.168.0.0/16
```
**Lưu ý:** `-p 80` chỉ quét cổng TCP 80. Sau đó liệt kê các dải IP hoặc subnet cần quét.

Full usage information can be found [tại đây](https://github.com/zmap/zmap/wiki).

![image](https://user-images.githubusercontent.com/100603074/210288512-fe050de5-fe7a-4c90-aab3-f307146f2b20.png)

*Image used from https://www.hackers-arise.com/post/zmap-for-scanning-the-internet-scan-the-entire-internet-in-45-minutes*

### [🔙](#tool-list)[**Shodan**]()

**Shodan** is a search engine for internet-connected devices.

It crawls the internet for assets, allowing users to search for specific devices and view information about them.

This information can include the device's IP address, the software and version it is running, and the type of device it is.

**Install:**

The search engine can be accessed at [https://www.shodan.io/dashboard](https://www.shodan.io/dashboard).
**Lưu ý:** Shodan là một dịch vụ trực tuyến, không cần cài đặt tool cục bộ (mặc dù có API và client CLI).

**Usage:**

[Nguyên tắc truy vấn Shodan](https://help.shodan.io/the-basics/search-query-fundamentals)

[Ví dụ truy vấn Shodan](https://www.shodan.io/search/examples)

[Cheat sheet truy vấn hay](https://www.osintme.com/index.php/2021/01/16/ultimate-osint-with-shodan-100-great-shodan-queries/)

![image](https://user-images.githubusercontent.com/100603074/191689282-70f99fe9-aa08-4cd3-b881-764eface8546.png)

*Image used from https://www.shodan.io/*

**Quản lý Lỗ hổng**
====================

*Các công cụ để nhận dạng, ưu tiên và giảm thiểu lỗ hổng trong mạng và trên từng thiết bị.*

### [🔙](#tool-list)[**OpenVAS**](https://openvas.org/)

**OpenVAS** is an open-source vulnerability scanner that helps identify security vulnerabilities in software and networks.

It is a tool that can be used to perform network security assessments and is often used to identify vulnerabilities in systems and applications so that they can be patched or mitigated.

**OpenVAS** is developed by the Greenbone Networks company and is available as a free and open-source software application.
**Lưu ý:** OpenVAS là một giải pháp quét lỗ hổng mạnh mẽ và miễn phí, là một phần của Greenbone Security Assistant.

**Install (Kali):**

```bash
apt-get update
apt-get dist-upgrade
apt-get install openvas
openvas-setup
```
**Lưu ý:** Các lệnh cài đặt và thiết lập **OpenVAS** trên **Kali Linux**. Lệnh `openvas-setup` sẽ thực hiện các bước cấu hình ban đầu, tải các feed lỗ hổng và tạo người dùng admin.

**Usage:**

```bash
openvas-start
```
**Lưu ý:** Lệnh khởi động các dịch vụ của **OpenVAS**.

Visit https://127.0.0.1:9392, accept the SSL certificate popup and login with admin credentials:

- username:admin
- password:(*Mật khẩu trong output lệnh openvas-setup*)
**Lưu ý:** Sau khi khởi động, bạn truy cập giao diện web của OpenVAS qua trình duyệt và đăng nhập bằng tài khoản admin đã tạo trong quá trình setup.

![image](https://user-images.githubusercontent.com/100603074/210452918-aa8d7be0-e557-4556-937c-334df02702dc.png)

*Image used from https://www.kali.org/blog/openvas-vulnerability-scanning/*

### [🔙](#tool-list)[**Nessus Essentials**](https://www.tenable.com/products/nessus/nessus-essentials)

**Nessus** is a vulnerability scanner that helps identify and assess the vulnerabilities that exist within a network or computer system.

It is a tool that is used to perform security assessments and can be used to identify vulnerabilities in systems and applications so that they can be patched or mitigated.

**Nessus** is developed by Tenable, Inc. and is available in both free and paid versions:

- The free version, called **Nessus Essentials**, is available for personal use only and is limited in its capabilities compared to the paid version.
- The paid version, called **Nessus Professional**, is more fully featured and is intended for use in a professional setting.
**Lưu ý:** Nessus là một trong những máy quét lỗ hổng phổ biến và được công nhận nhất trong ngành, do Tenable phát triển.

**Install:**

Register for a **Nessus Essentials** activation code [tại đây](https://www.tenable.com/products/nessus/nessus-essentials) and download.

Purchase **Nessus Professional** from [tại đây](https://www.tenable.com/products/nessus/nessus-professional).

**Usage:**

Extensive documentation can be found [tại đây](https://docs.tenable.com/nessus/Content/GetStarted.htm).

[Tìm kiếm **Plugin Nessus**](https://www.tenable.com/plugins/search)

[Cộng đồng Tenable](https://community.tenable.com/)

![image](https://user-images.githubusercontent.com/100603074/210452954-6208f96a-d180-4c8d-9579-313613d2cbe2.png)

*Image used from https://www.tenable.com*

### [🔙](#tool-list)[**Nexpose**](https://www.rapid7.com/products/nexpose/)

**Nexpose** is a vulnerability management tool developed by Rapid7. It is designed to help organizations identify and assess vulnerabilities in their systems and applications in order to mitigate risk and improve security.

**Nexpose** can be used to scan networks, devices, and applications in order to identify vulnerabilities and provide recommendations for remediation.

It also offers features such as asset discovery, risk prioritization, and integration with other tools in the Rapid7 vulnerability management platform.
**Lưu ý:** Nexpose là một giải pháp quản lý lỗ hổng của Rapid7, thường được dùng trong các môi trường doanh nghiệp lớn hơn, cung cấp tính năng phát hiện tài sản, ưu tiên rủi ro và tích hợp với các tool khác.

**Install:**

For detailed installation instructions see [tại đây](https://docs.rapid7.com/nexpose/install/).

**Usage:**

For full login information see [tại đây](https://docs.rapid7.com/nexpose/log-in-and-activate).

For usage and scan creation instructions see [tại đây](https://docs.rapid7.com/nexpose/create-and-scan-a-site).

![image](https://user-images.githubusercontent.com/100603074/210452992-cf9976ee-6b93-465d-bc1c-6e23cc387dba.png)

*Image used from https://www.rapid7.com/products/nexpose/*

### [🔙](#tool-list)[**HackerOne**](https://www.hackerone.com/)

**HackerOne** is a **bug bounty management company** that can be used to create and manage bug bounty programs for your business.

Bug bounty programs are a great way to outsource external vulnerability assessments, with the platform offering both private and public programs with the ability set program scopes and rules of engagement.

**HackerOne** also offer initial triage and management of external bug reports from researchers, with the ability to compensate researchers directly through the platform.
**Lưu ý:** Sử dụng các nền tảng bug bounty như HackerOne giúp Blue Team tận dụng sức mạnh cộng đồng ethical hacker để tìm ra các lỗ hổng bảo mật trên hạ tầng công cộng của mình mà có thể bị bỏ sót trong các bài kiểm tra pen test thông thường.

![image](https://user-images.githubusercontent.com/100603074/217382232-b8df098a-c74b-4552-b344-f5228c84c383.png)

*Image used from https://www.hackerone.com/product/bug-bounty-platform*

**Giám sát An ninh**
====================

*Các công cụ để thu thập và phân tích nhật ký bảo mật và các nguồn dữ liệu khác nhằm nhận dạng các mối đe dọa tiềm ẩn và hoạt động bất thường.*

### [🔙](#tool-list)[**Sysmon**](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon)

**Sysmon** is a **Windows system monitor** that tracks system activity and logs it to the **Windows event log**.

It provides detailed information about system activity, including process creation and termination, network connections, and changes to file creation time.

**Sysmon** can be configured to monitor specific events or processes and can be used to alert administrators of suspicious activity on a system.
**Lưu ý:** Sysmon là một công cụ cực kỳ giá trị cho Blue Team trên hệ thống Windows. Nó cung cấp logging ở mức độ hạt (granular logging) về hoạt động của tiến trình, kết nối mạng, tương tác với registry và filesystem, cho phép threat hunting và phát hiện các TTP tiên tiến hơn. Cần một cấu hình tốt (như Sysmon config của SwiftOnSecurity) để Sysmon hiệu quả và tránh tạo ra quá nhiều log.

**Install:**

Download the sysmon binary from [tại đây](https://download.sysinternals.com/files/Sysmon.zip).

**Cách sử dụng:**

```bash
# Cài đặt với cài đặt mặc định (image tiến trình được hash với SHA1 và không giám sát mạng)
sysmon -accepteula -i

# Cài đặt Sysmon với tệp cấu hình (như mô tả dưới đây)
sysmon -accepteula -i c:\windows\config.xml

# Gỡ cài đặt
sysmon -u

# Dump cấu hình hiện tại
sysmon -c
```
**Lưu ý:** Cài đặt Sysmon trên hệ thống Windows bằng các tham số dòng lệnh. `-i` để cài đặt, `-u` để gỡ cài đặt, `-c` để xem cấu hình hiện tại. Việc sử dụng `-i` với một tệp `.xml` (ví dụ `config.xml`) là cách phổ biến nhất để triển khai Sysmon với các bộ lọc event và hashing file được cấu hình trước.

Full event filtering information can be found [tại đây](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon#event-filtering-entries).

The Microsoft documentation page can be found [tại đây](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon).

![image](https://user-images.githubusercontent.com/100603074/210621009-b3c31c2b-f789-450a-acbf-7578fa943abd.png)

*Image used from https://nsaneforums.com/topic/281207-sysmon-5-brings-registry-modification-logging/*

### [🔙](#tool-list)[**Kibana**](https://www.elastic.co/kibana/)

**Kibana** is an open-source data visualization and exploration tool that is often used for log analysis in combination with **Elasticsearch**.

**Kibana** provides a user-friendly interface for searching, visualizing, and analyzing log data, which can be helpful for identifying patterns and trends that may indicate a security threat.

**Kibana** can be used to analyze a wide range of data sources, including system logs, network logs, and application logs. It can also be used to create custom dashboards and alerts to help security teams stay informed about potential threats and respond quickly to incidents.
**Lưu ý:** Kibana là giao diện người dùng cho Elastic Stack (trước đây là ELK). Blue Team sử dụng nó để trực quan hóa (dashboards, biểu đồ) và tìm kiếm (queries) một lượng lớn log tập trung (thường được thu thập bởi Logstash và lưu trữ trong Elasticsearch). Rất hữu ích cho việc giám sát, phân tích hành vi bất thường và threat hunting.

**Install:**

You can download **Kibana** from [tại đây](https://www.elastic.co/downloads/kibana).

Installation instructions can be found [tại đây](https://www.elastic.co/guide/en/kibana/current/install.html).

**Cách sử dụng (Trực quan hóa và khám phá dữ liệu log):**

**Kibana** cung cấp một loạt các công cụ trực quan hóa có thể giúp bạn nhận dạng các mẫu và xu hướng trong dữ liệu log của mình. Bạn có thể sử dụng các công cụ này để tạo dashboard tùy chỉnh hiển thị các chỉ số và cảnh báo liên quan.

**Cách sử dụng (Cảnh báo Đe dọa):**

**Kibana** có thể được cấu hình để gửi cảnh báo khi phát hiện các mẫu hoặc bất thường trong dữ liệu log của bạn. Bạn có thể thiết lập cảnh báo để thông báo về các mối đe dọa bảo mật tiềm ẩn, chẳng hạn như các lần đăng nhập thất bại hoặc kết nối mạng tới các địa chỉ IP độc hại đã biết.

Nice [blog](https://phoenixnap.com/kb/kibana-tutorial) about querying and visualizing data in **Kibana**.

![image](https://user-images.githubusercontent.com/100603074/210621061-badf3acf-2680-42c5-bbd9-43bca7a85cf2.png)

*Image used from https://www.pinterest.co.uk/pin/analysing-honeypot-data-using-kibana-and-elasticsearch--684758318328369269/*

### [🔙](#tool-list)[**Logstash**](https://www.elastic.co/logstash/)

**Logstash** is a open-source data collection engine with real-time pipelining capabilities. It is a server-side data processing pipeline that ingests data from a multitude of sources simultaneously, transforms it, and then sends it to a "stash" like **Elasticsearch**.

**Logstash** has a rich set of plugins, which allows it to connect to a variety of sources and process the data in multiple ways. It can parse and transform logs, translate data into a structured format, or send it to another tool for further processing.

With its ability to process large volumes of data quickly, **Logstash** is an integral part of the **ELK stack (Elasticsearch, Logstash, and Kibana)** and is often used to centralize, transform, and monitor log data.
**Lưu ý:** Logstash là thành phần xử lý trong Elastic Stack. Nó đóng vai trò là cầu nối giữa các nguồn log đa dạng (syslog, filebeat, agent, ...) và Elasticsearch. Blue Team cấu hình Logstash để thu thập, phân tích cú pháp (parse), làm sạch và chuẩn hóa dữ liệu log trước khi lưu trữ để tìm kiếm và phân tích dễ dàng hơn.

**Install:**

Download logstash from [tại đây](https://www.elastic.co/downloads/logstash).

**Usage:**

Full logstash documentation [tại đây](https://www.elastic.co/guide/en/logstash/current/introduction.html).

Configuration examples [tại đây](https://www.elastic.co/guide/en/logstash/current/config-examples.html).

![image](https://user-images.githubusercontent.com/100603074/210621111-e7630493-bc1c-41fa-af98-0261fbf6e293.png)

*Image used from https://www.elastic.co/guide/en/logstash/current/logstash-modules.html*

### [🔙](#tool-list)[**parsedmarc**](https://github.com/domainaware/parsedmarc)

A Python module and CLI utility for parsing DMARC reports.

When used with **Elasticsearch** and **Kibana** (or Splunk), it works as a self-hosted open source alternative to commercial DMARC report processing services such as Agari Brand Protection, Dmarcian, OnDMARC, ProofPoint Email Fraud Defense, and Valimail.
**Lưu ý:** DMARC là một tiêu chuẩn xác thực email giúp người nhận kiểm tra tính hợp lệ của email đến, ngăn chặn giả mạo nguồn gửi. DMARC cho phép chủ sở hữu domain nhận báo cáo về các email gửi đi sử dụng domain của họ. **parsedmarc** giúp xử lý các báo cáo DMARC này để phát hiện các email giả mạo.

Features:

- Parses draft and 1.0 standard aggregate/rua reports
- Parses forensic/failure/ruf reports
- Can parse reports from an inbox over IMAP, Microsoft Graph, or Gmail API
- Transparently handles gzip or zip compressed reports
- Consistent data structures
- Simple JSON and/or CSV output
- Optionally email the results
- Optionally send the results to Elasticsearch and/or Splunk, for use with premade dashboards
- Optionally send reports to Apache Kafka
**Lưu ý:** Các tính năng này giúp thu thập và xử lý báo cáo DMARC từ nhiều nguồn (email, API), giải nén, phân tích cú pháp và xuất ra các định dạng có cấu trúc (JSON/CSV), hoặc gửi thẳng đến SIEM (Elasticsearch, Splunk) hoặc Kafka để phân tích sâu hơn và hiển thị trên dashboard. Rất giá trị cho Blue Team để giám sát việc sử dụng domain của mình trong các chiến dịch phishing.

![image](https://user-images.githubusercontent.com/100603074/217382301-064ac450-3690-469d-9c86-c2e3c6cdeca9.png)

*Image used from https://github.com/domainaware/parsedmarc*

### [🔙](#tool-list)[**Phishing Catcher**](https://github.com/x0rz/phishing_catcher)

As a business, **phishing** can cause reputational and financial damage to you and your customers. Being able to proactively identify phishing infrastructure targeting your business helps to reduce the risk of these damages.
**Lưu ý:** Blue Team cần chủ động tìm kiếm các chiến dịch phishing sử dụng tên thương hiệu của tổ chức mình để cảnh báo người dùng hoặc yêu cầu gỡ bỏ các trang web độc hại.

**Phish catcher** allows you to catch possible phishing domains in near real time by looking for suspicious TLS certificate issuances reported to the **Certificate Transparency Log (CTL)** via the **CertStream API**.

"Suspicious" issuances are those whose domain name scores beyond a certain threshold based on a configuration file.
**Lưu ý:** Kỹ thuật Certificate Transparency Log ghi lại thông tin về mọi chứng chỉ TLS/SSL được cấp. **Phishing Catcher** theo dõi các log này, tìm kiếm các tên miền được cấp chứng chỉ mà giống tên miền của tổ chức (dùng các thuật toán so khớp mờ - fuzzy matching) và cảnh báo. Đây là phương pháp proactive để phát hiện hạ tầng phishing sớm.

![image](https://user-images.githubusercontent.com/100603074/217382453-400a044b-720d-47ce-adff-0a23e5511ae1.png)

*Image used from https://github.com/x0rz/phishing_catcher*

### [🔙](#tool-list)[**maltrail**](https://github.com/stamparm/maltrail)

**Maltrail** is a malicious traffic detection system, utilizing publicly available lists containing malicious and/or generally suspicious trails, along with static trails compiled from various AV reports and custom user defined lists. A trail can be anything from domain name, URL, IP address or HTTP User-Agent header value.
**Lưu ý:** Maltrail là một công cụ giám sát mạng (network monitoring tool) có thể hoạt động như một IDS/IPS dựa trên việc so sánh lưu lượng mạng với các chỉ báo độc hại (domain, IP, URL, User-Agent) từ các feed công khai hoặc tùy chỉnh.

A demo page for this tool can be found [tại đây](https://maltraildemo.github.io/).

**Install:**

```bash
sudo apt-get install git python3 python3-dev python3-pip python-is-python3 libpcap-dev build-essential procps schedtool
sudo pip3 install pcapy-ng
git clone --depth 1 https://github.com/stamparm/maltrail.git
cd maltrail
```
**Lưu ý:** Các lệnh cài đặt dependency hệ thống và thư viện Python, sau đó clone mã nguồn của **Maltrail**.

**Usage:**

```bash
sudo python3 sensor.py
```
**Lưu ý:** Lệnh chạy thành phần sensor của **Maltrail** để bắt đầu giám sát lưu lượng mạng. Cần quyền root (`sudo`) để truy cập raw packet.

![image](https://user-images.githubusercontent.com/100603074/217382540-fa1283d7-9825-4529-a92f-11f447e4657b.png)

*Image used from https://github.com/stamparm/maltrail*

### [🔙](#tool-list)[**AutorunsToWinEventLog**](https://github.com/palantir/windows-event-forwarding/tree/master/AutorunsToWinEventLog)

**Autoruns** is a tool developed by **Sysinternals** that allows you to view all of the locations in **Windows** where applications can insert themselves to launch at boot or when certain applications are opened. **Malware** often takes advantages of these locations to ensure that it runs whenever your computer boots up.
**Lưu ý:** Autoruns của Sysinternals liệt kê các vị trí **autorun** (nơi chương trình có thể tự khởi động cùng hệ thống). Đây là nơi phổ biến để malware thiết lập duy trì truy cập (persistence).

**Autoruns** conveniently includes a non-interactive command line utility. This code generates a CSV of Autoruns entries, converts them to JSON, and finally inserts them into a custom Windows Event Log. By doing this, we can take advantage of our existing **WEF** infrastructure to get these entries into our SIEM and start looking for signs of malicious persistence on endpoints and servers.
**Lưu ý:** Kỹ thuật này tự động chạy bản dòng lệnh của Autoruns (`Autorunsc`), thu thập thông tin về persistence, xử lý và ghi kết quả vào **Windows Event Log**. Điều này giúp tập trung hóa thông tin persistence vào SIEM thông qua Windows Event Forwarding (**WEF**), cho phép Blue Team giám sát hàng loạt máy tính để tìm dấu hiệu persistence độc hại mà không cần kiểm tra thủ công.

**Install:**

Download [**AutorunsToWinEventLog**](https://github.com/palantir/windows-event-forwarding/tree/master/AutorunsToWinEventLog).

**Usage:**

From an Admin Powershell console run `.\Install.ps1`

This script does the following:

- Creates the directory structure at c:\Program Files\AutorunsToWinEventLog
- Copies over AutorunsToWinEventLog.ps1 to that directory
- Downloads Autorunsc64.exe from https://live.sysinternals.com
- Sets up a scheduled task to run the script daily @ 11am
**Lưu ý:** **Script PowerShell Install.ps1** tự động hóa việc triển khai. Nó tạo thư mục, sao chép script chính, tải `Autorunsc64.exe` (bản dòng lệnh của Autoruns) và thiết lập một tác vụ theo lịch để chạy script thu thập dữ liệu định kỳ. Yêu cầu quyền quản trị viên để chạy script cài đặt này.

![image](https://user-images.githubusercontent.com/100603074/218199447-40e7add1-68ee-44e2-a297-3bf03c977a9c.png)

*Image used from https://www.detectionlab.network/usage/autorunstowineventlog/*

### [🔙](#tool-list)[**procfilter**](https://github.com/godaddy/procfilter)

**ProcFilter** is a process filtering system for **Windows** with built-in [YARA](https://github.com/virustotal/yara) integration. **YARA** rules can be instrumented with custom meta tags that tailor its response to rule matches. It runs as a Windows service and is integrated with [Microsoft's ETW API](https://msdn.microsoft.com/en-us/library/windows/desktop/bb968803%28v=vs.85%29.aspx), making results viewable in the **Windows Event Log**. Installation, activation, and removal can be done dynamically and does not require a reboot.
**Lưu ý:** ProcFilter hoạt động ở mức độ kernel (là một driver/service), giám sát và có thể ngăn chặn việc tạo/thực thi tiến trình dựa trên các quy tắc. Tích hợp **YARA** cho phép tạo các quy tắc phát hiện phức tạp dựa trên nội dung hoặc thuộc tính của file thực thi. Kết quả được ghi vào **Windows Event Log** thông qua **ETW** (Event Tracing for Windows).

**ProcFilter's** intended use is for **malware analysts** to be able to create **YARA signatures** that protect their Windows environments against a specific threat. It does not include a large signature set. Think lightweight, precise, and targeted rather than broad or all-encompassing. **ProcFilter** is also intended for use in controlled analysis environments where custom plugins can perform artifact-specific actions.
**Lưu ý:** Mục đích chính là cho các nhà phân tích **malware** (Blue Team) để tạo các quy tắc phát hiện/chặn rất cụ thể cho các mối đe dọa mới, thay vì một bộ quy tắc AV tổng quát. Nó hoạt động tốt trong các môi trường lab hoặc máy chủ nhạy cảm.

**Install:**

[ProcFilter x86/x64 Release/Debug Installers](https://github.com/godaddy/procfilter/releases)

*Note: Unpatched Windows 7 systems require hotfix 3033929 to load the driver component. More information can be found here.*

Nice configuration template file [tại đây](https://github.com/godaddy/procfilter/blob/master/files/procfilter.ini).

**Usage:**

```
procfilter -start
```
**Lưu ý:** Lệnh `procfilter -start` để bắt đầu service **ProcFilter**. Các tùy chọn khác thường là cài đặt service, dừng service, gỡ cài đặt, tải/tải lại file cấu hình (`procfilter.ini`). File cấu hình này chứa các quy tắc YARA và hành động khi quy tắc khớp (ví dụ: log, block).

Usage screenshots can be found [tại đây](https://github.com/godaddy/procfilter#screenshots).

![image](https://user-images.githubusercontent.com/100603074/218200282-f2465b93-169a-43d6-8e12-dea61ed9272c.png)

*Image used from https://github.com/godaddy/procfilter*

### [🔙](#tool-list)[**velociraptor**](https://github.com/Velocidex/velociraptor)

**Velociraptor** is a unique, advanced open-source **endpoint monitoring, digital forensic and cyber response platform**.

It was developed by **Digital Forensic and Incident Response (DFIR)** professionals who needed a powerful and efficient way to hunt for specific artifacts and monitor activities across fleets of endpoints. **Velociraptor** provides you with the ability to more effectively respond to a wide range of digital forensic and cyber incident response investigations and data breaches:
**Lưu ý:** Velociraptor là một nền tảng DFIR hiện đại. Nó cho phép thu thập dữ liệu pháp y từ xa, thực hiện threat hunting tự động trên nhiều máy cùng lúc và phản ứng nhanh với sự cố bằng cách chạy các "artefact" (quy trình thu thập dữ liệu tùy chỉnh). Rất mạnh mẽ cho Blue Team trong môi trường phân tán.

Features:

- Reconstruct attacker activities through **digital forensic analysis**
- Hunt for evidence of sophisticated adversaries
- Investigate malware outbreaks and other suspicious network activities
- Monitory continuously for suspicious user activities, such as files copied to **USB** devices
- Discover whether disclosure of confidential information occurred outside the network
- Gather endpoint data over time for use in **threat hunting** and future investigations
**Lưu ý:** Các tính năng chính của Velociraptor cho thấy khả năng ứng dụng rộng rãi trong các hoạt động của Blue Team: thu thập bằng chứng pháp y, threat hunting (chủ động tìm kiếm), giám sát hành vi người dùng (log USB...), và điều tra rò rỉ dữ liệu.

**Install:**

Download the binary from the [release page](https://github.com/Velocidex/velociraptor/releases).
**Lưu ý:** Có file binary độc lập cho nhiều hệ điều hành, dễ dàng triển khai thành agent hoặc server.

**Usage:**

```
velociraptor gui
```
**Lưu ý:** Lệnh chạy **Velociraptor** ở chế độ GUI (thường cho mục đích test hoặc server nhỏ).

Full usage information can be found [tại đây](https://docs.velociraptor.app/).

![image](https://user-images.githubusercontent.com/100603074/218200327-3f5ab599-11f1-46dc-8f28-b27c1258224a.png)

*Image used from https://docs.velociraptor.app*

### [🔙](#tool-list)[**SysmonSearch**](https://github.com/JPCERTCC/SysmonSearch)

**SysmonSearch** makes event log analysis more effective and less time consuming, by aggregating event logs generated by **Microsoft's Sysmon**.
**Lưu ý:** **SysmonSearch** là một giải pháp bổ sung để phân tích log Sysmon. Thay vì chỉ xem log thô, nó giúp tập trung và phân tích.

**SysmonSearch** uses Elasticserach and **Kibana** (and Kibana plugin).
  * **Elasticserach**
    **Elasticsearch** collects/stores Sysmon's event log.
  * **Kibana**
    **Kibana** provides user interface for your Sysmon's event log analysis. The following functions are implemented as **Kibana plugin**.
    * Visualizes Function
      This function visualizes **Sysmon's** event logs to illustrate correlation of processes and networks.
    * Statistical Function
      This function collects the statistics of each device or **Sysmon's event ID**.
    * Monitor Function
      This function monitor incoming logs based on the preconfigured rules, and trigers alert.
  * **StixIoC server**
    You can add search/monitor condition by uploading STIX/IOC file. From **StixIoC server Web UI**, you can upload STIXv1, STIXv2 and OpenIOC format files.
**Lưu ý:** **SysmonSearch** tích hợp với Elastic Stack (**Elasticsearch, Kibana**) và thêm các tính năng chuyên biệt để phân tích log **Sysmon** hiệu quả hơn (trực quan hóa mối liên hệ tiến trình/mạng, thống kê, giám sát và cảnh báo). Nó cũng hỗ trợ import IoC từ các định dạng chuẩn như STIX và OpenIOC.

**Install (Linux):**

```bash
git clone https://github.com/JPCERTCC/SysmonSearch.git
```
**Lưu ý:** Clone mã nguồn. Cần cài đặt Elastic Stack trước đó.

[Modify Elasticsearch configuration](https://github.com/JPCERTCC/SysmonSearch/wiki/Install#elasticsearch-server-setup)

[Modify Kibana configuration](https://github.com/JPCERTCC/SysmonSearch/wiki/Install#kibana-server-setup)

Full installation instructions can be found [tại đây](https://github.com/JPCERTCC/SysmonSearch/wiki/Install).

**Cách sử dụng:**

*Once Elasticsearch and Kibana configurations have been modified, restart the services and navigate to your **Kibana interface**. The **SysmonSearch ribbon** should be visible.*

[Visualize the Sysmon log to investigate suspicious behavior](https://blogs.jpcert.or.jp/ja/2018/09/SysmonSearch.html)

![image](https://user-images.githubusercontent.com/100603074/218200383-84e4c9f4-3e34-4973-b37c-a9160a74b5e0.png)

*Image used from https://blogs.jpcert.or.jp/ja/2018/09/SysmonSearch.html*

**Công cụ và Kỹ thuật Đe dọa**
====================

*Các công cụ để nhận dạng và triển khai các biện pháp phát hiện chống lại các TTP được sử dụng bởi các tác nhân đe dọa.*

### [🔙](#tool-list)[**lolbas-project.github.io**](https://lolbas-project.github.io/)

Living off the land binaries (**LOLBins**) are legitimate Windows executables that can be used by threat actors to carry out malicious activities without raising suspicion.

Using **LOLBins** allows attackers to blend in with normal system activity and evade detection, making them a popular choice for malicious actors.
**Lưu ý:** LOLBins là các tệp thực thi hoặc script của hệ thống Windows được thiết kế để thực hiện các tác vụ hợp pháp, nhưng kẻ tấn công lạm dụng chúng cho mục đích độc hại (ví dụ: `certutil.exe` để tải file, `bitsadmin.exe` để truyền file, `cscript.exe` để chạy script...). Chúng khó bị phát hiện bằng các giải pháp bảo mật truyền thống dựa trên chữ ký.

The **LOLBAS project** is a MITRE mapped list of **LOLBINS** with commands, usage and detection information for defenders.
**Lưu ý:** Project LOLBAS (Living Off a Little Bit Susi) thu thập và tài liệu hóa cách các binary/script hệ thống Windows bị lạm dụng, cung cấp thông tin cho Blue Team để hiểu TTP này và tạo các quy tắc phát hiện dựa trên dòng lệnh, kết nối mạng, hoặc hành vi bất thường của các LOLBins. Ánh xạ với framework **MITRE ATT&CK**.

Visit [https://lolbas-project.github.io/](https://lolbas-project.github.io/).

**Usage:**

Use the information for detection opportunities to harden your infrastructure against **LOLBIN usage**.

Here are some project links to get started:

- [Bitsadmin.exe](https://lolbas-project.github.io/lolbas/Binaries/Bitsadmin/)
- [Certutil.exe](https://lolbas-project.github.io/lolbas/Binaries/Certutil/)
- [Cscript.exe](https://lolbas-project.github.io/lolbas/Binaries/Cscript/)
**Lưu ý:** Bạn nên duyệt các trang này để xem các lệnh cụ thể mà attacker sử dụng với từng binary, từ đó tạo ra các cảnh báo trong SIEM hoặc EDR (ví dụ: alert khi certutil.exe thực thi với đối số liên quan đến tải file từ URL).

![image](https://user-images.githubusercontent.com/100603074/210625466-9ab87233-e822-4961-a68a-f863f56ef830.png)

*Image used from https://lolbas-project.github.io/*

### [🔙](#tool-list)[**gtfobins.github.io**](https://gtfobins.github.io/)

**GTFOBins** (short for "Get The F* Out Binaries") is a collection of Unix binaries that can be used to escalate privileges, bypass restrictions, or execute arbitrary commands on a system.
**Lưu ý:** GTFOBins tương tự như LOLBAS nhưng dành cho hệ thống Linux/Unix. Nó tập hợp các binary (wget, curl, vi, awk...) có sẵn trên hầu hết các hệ thống Linux có thể bị lạm dụng cho các mục đích tấn công như thoát khỏi môi trường bị giới hạn (shell bị giới hạn), bypass `sudo`, thực thi lệnh tùy ý...

They can be used by threat actors to gain unauthorized access to systems and carry out malicious activities.

The **GTFOBins** project is a list of Unix binaries with command and usage information for attackers. This information can be used to implement unix detections.
**Lưu ý:** Mặc dù trang web trình bày từ góc độ attacker, Blue Team sử dụng nó để hiểu các kỹ thuật lạm dụng các binary Linux và tạo các quy tắc phát hiện cho môi trường Linux của mình.

Visit [https://gtfobins.github.io/](https://gtfobins.github.io/).

**Usage:**

Here are some project links to get started:

- [base64](https://gtfobins.github.io/gtfobins/base64/)
- [curl](https://gtfobins.github.io/gtfobins/curl/)
- [nano](https://gtfobins.github.io/gtfobins/nano/)
**Lưu ý:** Blue Team xem các trang của từng binary để thấy các lệnh cụ thể mà attacker dùng (ví dụ: cách dùng `base64` để thực thi lệnh từ chuỗi base64, cách dùng `curl` để upload/download file theo cách lén lút, cách dùng các text editor như `nano` để thoát khỏi shell giới hạn), sau đó tạo detection rules.

![image](https://user-images.githubusercontent.com/100603074/210625527-6a037b81-e3fe-4282-a193-1cc4b9c06f75.png)

*Image used from https://gtfobins.github.io/*

### [🔙](#tool-list)[**filesec.io**](https://filesec.io/)

**Filesec** is a list of file extensions that can be used by attackers for **phishing, execution, macros** etc.

This is a nice resource to understand the malicious use cases of common file extentions and ways that you can defend against them.

Each file extension page contains a description, related operating system and recommendations.
**Lưu ý:** Blue Team nên tham khảo nguồn này để hiểu các rủi ro liên quan đến từng loại phần mở rộng file (đặc biệt là các loại ít phổ biến hoặc thường bị lạm dụng) và cách phòng vệ (ví dụ: chặn file loại đó ở cổng email/proxy, cấu hình chính sách hạn chế thực thi file theo loại).

Visit [https://filesec.io/](https://filesec.io/).

**Usage:**

Here are some project links to get started:

- [.Docm](https://filesec.io/docm)
- [.Iso](https://filesec.io/iso)
- [.Ppam](https://filesec.io/ppam)
**Lưu ý:** Mỗi trang về một phần mở rộng file cung cấp thông tin về rủi ro và các biện pháp phòng vệ liên quan đến nó.

![image](https://user-images.githubusercontent.com/100603074/210625626-58223992-2821-42c6-878a-e6aea4b9a508.png)

*Image used from https://filesec.io/*

### [🔙](#tool-list)[**KQL Search**](https://www.kqlsearch.com/)

**KQL** stands for "**Kusto Query Language**", and it is a query language used to search and filter data in **Azure Monitor** logs. It is similar to SQL, but is more optimized for log analytics and time-series data.
**Lưu ý:** KQL được sử dụng rộng rãi trong các dịch vụ logging và phân tích của Microsoft như Azure Monitor, Azure Sentinel/Microsoft Sentinel, và Application Insights.

**KQL query language** is particularly useful for blue teamers because it allows you to quickly and easily search through large volumes of log data to identify security events and anomalies that may indicate a threat.

**KQL Search** is a web app created by [@ugurkocde](https://twitter.com/ugurkocde) that aggregates **KQL queries** that are shared on GitHub.
**Lưu ý:** Đây là một nguồn tài nguyên hữu ích để Blue Team tìm các truy vấn KQL đã được cộng đồng chia sẻ để phát hiện các TTP, lỗ hổng, hoặc các hành vi độc hại trong log Azure/Windows.

You can visit the site at [https://www.kqlsearch.com/](https://www.kqlsearch.com/).

More information about **Kusto Query Language (KQL)** can be found [tại đây](https://learn.microsoft.com/en-us/azure/data-explorer/kusto/query/).

![image](https://user-images.githubusercontent.com/100603074/210736862-1e0cf987-7c85-40c1-b51c-1f3a1f946f7d.png)

*Image used from https://www.kqlsearch.com/*

### [🔙](#tool-list)[**Unprotect Project**](https://unprotect.it/about/)

Malware authors spend a great deal of time and effort to develop complex code to perform malicious actions against a target system. It is crucial for malware to remain undetected and avoid sandbox analysis, antiviruses or malware analysts.

With this kind of technics, **malware** are able to pass under the radar and stay undetected on a system. The goal of this free database is to centralize the information about **malware evasion techniques**.
**Lưu ý:** **Unprotect Project** tập trung vào các kỹ thuật mà malware sử dụng để né tránh bị phát hiện (bởi AV, EDR, sandbox) và né tránh bị phân tích (bởi malware analyst).

The project aims to provide **Malware Analysts and Defenders** with actionable insights and detection capabilities to shorten their response times.
**Lưu ý:** Thông tin này rất hữu ích cho Blue Team và các nhà phân tích **malware** để hiểu cách các phần mềm độc hại hiện đại ẩn mình, từ đó cải thiện các biện pháp phòng vệ (tạo detection logic tinh vi hơn, cấu hình sandbox hiệu quả hơn,...) và đẩy nhanh quá trình ứng phó.

The project can be found at [https://unprotect.it/](https://unprotect.it/).

The project has an **API** - Docs [tại đây](https://unprotect.it/api/).

![image](https://user-images.githubusercontent.com/100603074/210743650-6adaddce-ecb3-41bb-854b-292482b73d55.png)

*Image used from https://unprotect.it/map/*

### [🔙](#tool-list)[**chainsaw**](https://github.com/WithSecureLabs/chainsaw)

**Chainsaw** provides a powerful ‘first-response’ capability to quickly identify threats within **Windows forensic artefacts** such as **Event Logs** and MFTs. **Chainsaw** offers a generic and fast method of searching through **event logs** for keywords, and by identifying threats using built-in support for **Sigma detection rules**, and via custom **Chainsaw** detection rules.
**Lưu ý:** Chainsaw là một công cụ phân tích log và forensic nhanh trên hệ thống Windows, tập trung vào Event Logs (EVTX) và MFT (Master File Table). Điểm mạnh là tốc độ và tích hợp với luật **Sigma** - một định dạng chuẩn để viết luật phát hiện TTP.

Features:

- Hunt for threats using **Sigma detection rules** and custom **Chainsaw detection rules**
- Search and extract **forensic artefacts** by string matching, and regex patterns
- Lightning fast, written in rust, wrapping the **EVTX parser library** by @OBenamram
- Clean and lightweight execution and output formats without unnecessary bloat
- Document tagging (detection logic matching) provided by the **TAU Engine Library**
- Output results in a variety of formats, such as ASCII table format, CSV format, and JSON format
- Can be run on **MacOS, Linux** and **Windows**
**Lưu ý:** Các tính năng cho thấy Chainsaw mạnh mẽ cho threat hunting và phân tích sự cố: tìm kiếm dựa trên luật phát hiện (Sigma, Chainsaw), trích xuất dữ liệu dựa trên pattern, xử lý log EVTX nhanh chóng, hỗ trợ nhiều định dạng output. Khả năng chạy trên nhiều HĐH là một lợi thế.

**Install:**

```bash
git clone https://github.com/countercept/chainsaw.git
cargo build --release
git clone https://github.com/SigmaHQ/sigma
git clone https://github.com/sbousseaden/EVTX-ATTACK-SAMPLES.git
```
**Lưu ý:** Tải mã nguồn **Chainsaw** bằng **Git**, biên dịch nó bằng **Cargo** (trình quản lý gói Rust), và tải thêm các repository chứa luật **Sigma** và các mẫu Event Log tấn công (để test hoặc làm quen).

**Usage:**

```bash
./chainsaw hunt EVTX-ATTACK-SAMPLES/ -s sigma/ --mapping mappings/sigma-event-logs-all.yml
```
**Lưu ý:** Ví dụ sử dụng `chainsaw hunt` để tìm kiếm các dấu hiệu tấn công trong các file Event Log mẫu (`EVTX-ATTACK-SAMPLES/`) sử dụng các luật **Sigma** (`-s sigma/`) và file ánh xạ (mapping file).

![image](https://user-images.githubusercontent.com/100603074/217382675-1834c13d-1789-4ea7-a46e-25808477bcf0.png)

*Image used from https://twitter.com/FranticTyping/status/1433386064429916162/*

### [🔙](#tool-list)[**freq**](https://github.com/MarkBaggett/freq)

Adversaries attempt to bypass signature based/pattern matching/blacklist techniques by introducing random: filenames, service names, workstation names, domains, hostnames, SSL cert subjects and issuer subjects, etc.
**Lưu ý:** Kỹ thuật tạo tên ngẫu nhiên cho file, domain,... được **malware** và attacker sử dụng để tránh bị phát hiện bằng các biện pháp dựa trên blacklist hoặc pattern tĩnh. Việc phân tích entropy của chuỗi có thể giúp phát hiện.

**Freq** is a python API designed by Mark Baggett to handle mass entropy testing. It was designed to be used in conjunction with a SIEM solutions but can work with anything that can submit a web request.

The tool uses frequency tables that map how likely one character will follow another
**Lưu ý:** Freq phân tích khả năng ngẫu nhiên (entropy) của các chuỗi (đặc biệt là tên domain, hostname,...) dựa trên tần suất xuất hiện của các ký tự và sự kết hợp của chúng trong ngôn ngữ tự nhiên. Entropy cao hơn bình thường có thể là dấu hiệu của thuật toán tạo domain (**DGA**), một kỹ thuật **malware** dùng để liên lạc với **C2**.

**Install:**

```bash
git clone https://github.com/MarkBaggett/freq
cd freq
```
**Lưu ý:** Cài đặt bằng Git. Freq là một **package/script Python**.

**Usage:**

```bash
# Running freq_server.py on port 10004 and using a frequency table of /opt/freq/dns.freq
/usr/bin/python /opt/freq/freq_server.py 10004 /opt/freq/dns.freq
```
**Lưu ý:** Ví dụ chạy server Freq. Công cụ này có thể được tích hợp vào SIEM bằng cách gửi các chuỗi cần kiểm tra đến server Freq thông qua API, sau đó SIEM xử lý kết quả. File `dns.freq` là một file dữ liệu chứa tần suất xuất hiện ký tự/cặp ký tự trong các tên domain hợp lệ để dùng làm tham chiếu.

### [🔙](#tool-list)[**yarGen**](https://github.com/Neo23x0/yarGen)

**yarGen** is a generator for YARA rules
**Lưu ý:** **YARA** là công cụ giúp nhận dạng malware dựa trên các luật (chứa chuỗi ký tự, pattern binary...). **yarGen** giúp tự động hóa quá trình viết các luật YARA này.

The main principle is the creation of **yara rules** from strings found in malware files while removing all strings that also appear in goodware files. Therefore **yarGen** includes a big goodware strings and opcode database as ZIP archives that have to be extracted before the first use.

The rule generation process also tries to identify similarities between the files that get analyzed and then combines the strings to so called super rules. The super rule generation does not remove the simple rule for the files that have been combined in a single super rule. This means that there is some redundancy when super rules are created. You can suppress a simple rule for a file that was already covered by super rule by using `--nosimple`.
**Lưu ý:** **yarGen** so sánh các chuỗi/pattern trong các mẫu malware với cơ sở dữ liệu các chuỗi/pattern từ "goodware" (phần mềm hợp pháp) để tạo ra các luật YARA chỉ chứa các yếu tố duy nhất có trong malware, giảm thiểu cảnh báo sai (false positives). Nó cũng cố gắng gom các luật từ các malware tương tự lại thành "super rules".

**Install:**

Download the latest [release](https://github.com/Neo23x0/yarGen/releases).

```bash
pip install -r requirements.txt
python yarGen.py --update
```
**Lưu ý:** Cài đặt các dependency Python và sau đó cập nhật cơ sở dữ liệu goodware của **yarGen** bằng **script Python yarGen.py**.

**Usage:**

```bash
# Create a new strings and opcodes database from an Office 2013 program directory
yarGen.py -c --opcodes -i office -g /opt/packs/office2013

# Update the once created databases with the "-u" parameter
yarGen.py -u --opcodes -i office -g /opt/packs/office365
```
**Lưu ý:** Các ví dụ về cách sử dụng **script Python yarGen.py** để tạo (`-c`) hoặc cập nhật (`-u`) cơ sở dữ liệu goodware/opcodes bằng cách chỉ định loại software (`-i`) và thư mục chứa các file của phần mềm đó (`-g`). Điều này giúpyarGen học từ môi trường phần mềm hợp pháp cụ thể trong tổ chức để tạo luật chính xác hơn.

Usage examples can be found [tại đây](https://github.com/Neo23x0/yarGen#examples).

![image](https://user-images.githubusercontent.com/100603074/218200487-8476950d-c63e-4d5a-a03c-f2969b6001cc.png)

*Image used from https://github.com/Neo23x0/yarGen*

### [🔙](#tool-list)[**EmailAnalyzer**](https://github.com/keraattin/EmailAnalyzer)

With **EmailAnalyzer** you can able to analyze your suspicious emails. You can extract headers, links and hashes from the .eml file
**Lưu ý:** Công cụ này hỗ trợ phân tích ban đầu các email đáng ngờ được lưu dưới dạng file `.eml`.

**Install:**

```bash
git clone https://github.com/keraattin/EmailAnalyzer
cd EmailAnalyzer
```
**Lưu ý:** Cài đặt bằng Git. Đây là một **script Python**.

**Usage:**

```bash
# View headers in eml file
python3 email-analyzer.py -f <eml file> --headers

# Get hashes
python3 email-analyzer.py -f <eml file> --digests

# Get links
python3 email-analyzer.py -f <eml file> --links

# Get attachments
python3 email-analyzer.py -f <eml file> --attachments
```
**Lưu ý:** Các ví dụ sử dụng **script Python email-analyzer.py** với cờ `-f` chỉ định file `.eml` và các cờ khác (`--headers`, `--digests`, `--links`, `--attachments`) để trích xuất thông tin khác nhau từ email. Hữu ích cho Blue Team khi phân tích email phishing hoặc email chứa mã độc để lấy IOC.

![image](https://user-images.githubusercontent.com/100603074/218200574-d9917b8c-433b-4bab-8db0-b6628b0d9424.png)

*Text used from https://github.com/keraattin/EmailAnalyzer*

### [🔙](#tool-list)[**VCG**](https://github.com/nccgroup/VCG)

**VCG** is an automated **code security review tool** that handles **C/C++, Java, C#, VB** and PL/SQL. It has a few features that should hopefully make it useful to anyone conducting code security reviews, particularly where time is at a premium:
**Lưu ý:** VCG (Vulnerability Code Grep?) là công cụ phân tích mã nguồn tĩnh tự động để tìm các lỗ hổng bảo mật trong nhiều ngôn ngữ lập trình. Blue Team có thể dùng nó để kiểm tra mã nguồn các ứng dụng nội bộ hoặc third-party được deploy.

- In addition to performing some more complex checks it also has a config file for each language that basically allows you to add any bad functions (or other text) that you want to search for
- It attempts to find a range of around 20 phrases within comments that can indicate broken code (“ToDo”, “FixMe”, “Kludge”, etc.)
- It provides a nice pie chart (for the entire codebase and for individual files) showing relative proportions of code, whitespace, comments, ‘ToDo’ style comments and bad code
**Lưu ý:** Tính năng nổi bật bao gồm khả năng tùy chỉnh luật tìm kiếm hàm/text độc hại, tìm kiếm các comment "Todo" hoặc "Fixme" (đôi khi liên quan đến các vấn đề chưa được giải quyết hoặc các chỗ mã yếu) và tạo báo cáo trực quan.

**Install:**

You can install the pre-compiled binary [tại đây](https://github.com/nccgroup/VCG).
**Lưu ý:** Tải file binary đã biên dịch sẵn.

Open the project .sln, choose "**Release**", and **build**.
**Lưu ý:** Biên dịch mã nguồn C# bằng Visual Studio (nếu muốn build từ source).

**Usage:**

```
STARTUP OPTIONS:
	(Set desired starting point for GUI. If using console mode these options will set target(s) to be scanned.)
	-t, --target <Filename|DirectoryName>:	Set target file or directory. Use this option either to load target immediately into GUI or to provide the target for console mode.
	-l, --language <CPP|PLSQL|JAVA|CS|VB|PHP|COBOL>:	Set target language (Default is C/C++).
	-e, --extensions <ext1|ext2|ext3>:	Set file extensions to be analysed (See ReadMe or Options screen for language-specific defaults).
	-i, --import <Filename>:	Import XML/CSV results to GUI.

OUTPUT OPTIONS:
	(Automagically export results to a file in the specified format. Use XML or CSV output if you wish to reload results into the GUI later on.)
	-x, --export <Filename>:	Automatically export results to XML file.
	-f, --csv-export <Filename>:	Automatically export results to CSV file.
	-r, --results <Filename>:	Automatically export results to flat text file.

CONSOLE OPTIONS:
	-c, --console:		Run application in console only (hide GUI).
	-v, --verbose:		Set console output to verbose mode.
	-h, --help:		Show help.
```
**Lưu ý:** Output màn hình trợ giúp của VCG, liệt kê các tham số dòng lệnh cho cả chế độ GUI và console.

### [🔙](#tool-list)[**CyberChef**](https://gchq.github.io/CyberChef/)

**CyberChef** is a free, web-based tool that allows users to manipulate and transform data using a wide range of techniques.

With **CyberChef**, you can perform a wide range of operations on data, such as converting between different data formats (e.g., hexadecimal, base64, ASCII), encoding and decoding data, searching and replacing text etc.

The tool also includes a recipe system, which allows you to save and share data manipulation workflows with others.
**Lưu ý:** CyberChef được ví như "con dao quân đội Thụy Sĩ" cho các công tác xử lý dữ liệu. Blue Team sử dụng nó thường xuyên trong phân tích malware, phân tích network traffic, xử lý các chuỗi độc hại, decode/encode các định dạng khác nhau trong quá trình điều tra sự cố.

The tool can be used from [tại đây](https://gchq.github.io/CyberChef/).

![image](https://user-images.githubusercontent.com/100603074/223865168-433fcd56-12e9-44a2-83aa-1531d711383d.png)

*Image used from https://gchq.github.io/CyberChef/*

**Tình báo Đe dọa**
====================

*Các công cụ để thu thập và phân tích tình báo về các mối đe dọa hiện tại và mới nổi, và để tạo cảnh báo về các mối đe dọa tiềm ẩn.*

### [🔙](#tool-list)[**Maltego**](https://www.maltego.com/solutions/cyber-threat-intelligence/)

**Maltego** is a commercial **threat intelligence and forensics tool** developed by Paterva. It is used by security professionals to gather and analyze information about domains, IP addresses, networks, and individuals in order to identify relationships and connections that might not be immediately apparent.

**Maltego** uses a visual interface to represent data as entities, which can be linked together to form a network of relationships. It includes a range of transforms, which are scripts that can be used to gather data from various sources, such as social media, **DNS** records, and **WHOIS** data.

**Maltego** is often used in conjunction with other security tools, such as SIEMs and vulnerability scanners, as part of a comprehensive **threat intelligence and incident response strategy**.
**Lưu ý:** Maltego giúp Blue Team vẽ bản đồ mối liên hệ giữa các thực thể (địa chỉ IP, domain, email, tên người, tổ chức, file hash...) để hiểu rõ hơn về kẻ tấn công, hạ tầng C2, hoặc mạng lưới tấn công trong quá trình phân tích sự cố và threat hunting.

You can schedule a demo [tại đây](https://www.maltego.com/get-a-demo/).

[Maltego handbook Handbook for Cyber Threat Intelligence](https://static.maltego.com/cdn/Handbooks/Maltego-Handbook-for-Cyber-Threat-Intelligence.pdf)

![image](https://user-images.githubusercontent.com/100603074/210655712-e1409206-de1d-4601-88a5-f5a6ac3928c7.png)

*Image used from https://www.maltego.com/reduce-your-cyber-security-risk-with-maltego/*

### [🔙](#tool-list)[**MISP**](https://www.misp-project.org/)

**MISP** (short for **Malware Information Sharing Platform**) is an open-source platform for sharing, storing, and correlating **Indicators of Compromise (IOCs)** of targeted attacks, threats, and malicious activity.
**Lưu ý:** MISP là nền tảng chia sẻ và quản lý thông tin tình báo đe dọa (Threat Intelligence Platform - TIP). Nó cho phép Blue Team nhập, xuất, chia sẻ (với cộng đồng hoặc nhóm riêng), và tự động tương quan (correlation) các IoC như hash file, địa chỉ IP, domain, email address...

**MISP** includes a range of features, such as real-time sharing of **IOCs**, support for multiple formats, and the ability to import and export data to and from other tools.

It also provides a RESTful API and various data models to facilitate the integration of **MISP** with other security systems. In addition to its use as a **threat intelligence platform, MISP** is also used for **incident response, forensic analysis, and malware research**.
**Lưu ý:** Việc tích hợp MISP với SIEM, EDR, firewall giúp tự động chặn các IoC hoặc tạo cảnh báo khi các IoC này xuất hiện trong log hệ thống.

**Install:**

```bash
# Kali
wget -O /tmp/misp-kali.sh https://raw.githubusercontent.com/MISP/MISP/2.4/INSTALL/INSTALL.sh && bash /tmp/misp-kali.sh

# Ubuntu 20.04.2.0-server
wget -O /tmp/INSTALL.sh https://raw.githubusercontent.com/MISP/MISP/2.4/INSTALL/INSTALL.sh
bash /tmp/INSTALL.sh
```
**Lưu ý:** Các lệnh cài đặt MISP trên hệ thống Linux (Kali hoặc Ubuntu) bằng cách tải và chạy script cài đặt chính thức. Việc cài đặt MISP khá phức tạp, thường cần cấu hình database và web server.

Full installation instructions can be found [tại đây](https://misp.github.io/MISP/).

**Usage:**

**MISP** documentation can be found [tại đây](https://www.misp-project.org/documentation/).

[Hướng dẫn sử dụng MISP](https://github.com/MISP/misp-book)

[**MISP** Training Cheat sheet](https://www.misp-project.org/misp-training/cheatsheet.pdf)

![image](https://user-images.githubusercontent.com/100603074/210655743-b7fd5ab0-a106-4277-815d-c674525a9a91.png)

*Image used from http://www.concordia-h2020.eu/blog-post/integration-of-misp-into-flowmon-ads/*

### [🔙](#tool-list)[**ThreatConnect**](https://threatconnect.com/threat-intelligence-platform/)

**ThreatConnect** is a **threat intelligence platform** that helps organizations aggregate, analyze, and act on threat data. It is designed to provide a single, unified view of an organization's threat landscape and enable users to collaborate and share information about threats.
**Lưu ý:** ThreatConnect là một nền tảng TIP thương mại tương tự MISP, giúp tổng hợp, phân tích và chia sẻ thông tin tình báo về đe dọa, hỗ trợ phối hợp ứng phó.

The platform includes a range of features for collecting, analyzing, and disseminating threat intelligence, such as a customizable dashboard, integration with third-party data sources, and the ability to create custom reports and alerts.

It is intended to help organizations improve their security posture by providing them with the information they need to identify, prioritize, and respond to potential threats.
**Lưu ý:** Việc tích hợp nhiều nguồn threat intelligence khác nhau (feed công khai, thương mại, chia sẻ từ cộng đồng) và khả năng tạo các workflow phân tích/phản ứng là điểm mạnh của các nền tảng TIP như ThreatConnect.

You can request a demo from [tại đây](https://threatconnect.com/request-a-demo/).

[**ThreatConnect** for Threat Intel Analysts - PDF](https://threatconnect.com/wp-content/uploads/2022/12/Intel-Analysts-Datasheet.pdf)

![image](https://user-images.githubusercontent.com/100603074/210655770-4413ead0-6216-47fe-a933-cbe0be9f86a1.png)

*Image used from https://threatconnect.com/threat-intelligence-platform/*

### [🔙](#tool-list)[**Adversary Emulation Library**](https://github.com/center-for-threat-informed-defense/adversary_emulation_library)

This is a library of adversary emulation plans to enable you to evaluate your defensive capabilities against real-world threats.

Emulation plans are an essential component for organizations looking to prioritize defenses against behavior from specific threats.
**Lưu ý:** Thư viện này không phải là phần mềm hay công cụ thực thi, mà là bộ tài liệu (kế hoạch chi tiết) để Blue Team (hoặc Purple Team) có thể mô phỏng lại các TTP của các nhóm tấn công thực tế đã biết (Adversary Emulation) để kiểm tra hiệu quả của các biện pháp phòng vệ hiện có.

The TTPs outlined in this resource can be used to design specific threat emulation activities to test your organisations defenses against specific threat actors.
**Lưu ý:** Blue Team sử dụng các kế hoạch trong thư viện này để hiểu sâu hơn về các kỹ thuật (TTP) mà các nhóm tấn công nổi tiếng sử dụng và tái tạo chúng trong môi trường test để xem hệ thống giám sát/phòng thủ có phát hiện hoặc ngăn chặn được không.

Visit the resource [tại đây](https://github.com/center-for-threat-informed-defense/adversary_emulation_library).

**Example (sandworm)**

- [Mã nguồn Phần mềm Mô phỏng Sandworm](https://github.com/center-for-threat-informed-defense/adversary_emulation_library/tree/master/sandworm/Resources)
- [Hướng dẫn Chi tiết Kịch bản Phát hiện Sandworm](https://github.com/center-for-threat-informed-defense/adversary_emulation_library/tree/master/sandworm/Emulation_Plan/Scenario_1)
- [Tóm tắt Thông tin Tình báo Sandworm](https://github.com/center-for-threat-informed-defense/adversary_emulation_library/blob/master/sandworm/Intelligence_Summary/Intelligence_Summary.md)
**Lưu ý:** Các ví dụ cụ thể cho một nhóm tấn công (Sandworm), cung cấp mã nguồn công cụ để thực thi mô phỏng, hướng dẫn cách thiết lập môi trường test, thực hiện các bước mô phỏng, và cách kiểm tra xem các giải pháp bảo mật có phát hiện được hay không. Rất chi tiết và thực tế cho việc nâng cao khả năng phòng thủ dựa trên threat intelligence.

![image](https://user-images.githubusercontent.com/100603074/223865356-c4d491c3-edba-40d6-80b2-5c41029bddfd.png)

*Image used from https://github.com/center-for-threat-informed-defense/adversary_emulation_library*

**Lập kế hoạch Ứng phó Sự cố**
====================

*Các công cụ để tạo và duy trì kế hoạch ứng phó sự cố, bao gồm các mẫu và các thực hành tốt nhất để ứng phó với các loại sự cố khác nhau.*

### [🔙](#tool-list)[**NIST**](https://www.nist.gov/cyberframework)

The **NIST Cybersecurity Framework (CSF)** is a framework developed by the **National Institute of Standards and Technology (NIST)** to help organizations manage cybersecurity risks. It provides a set of guidelines, best practices, and standards for implementing and maintaining a robust cybersecurity program.
**Lưu ý:** Khung NIST CSF là một tài liệu tham khảo quan trọng cho Blue Team để xây dựng một chương trình bảo mật toàn diện, không chỉ riêng ứng phó sự cố mà còn cả nhận diện, bảo vệ, phát hiện và phục hồi.

The framework is organized around five core functions: Identify, Protect, Detect, Respond, and Recover. These functions provide a structure for understanding and addressing the various components of cybersecurity risk.

The **CSF** is designed to be flexible and adaptable, and it can be customized to fit the specific needs and goals of an organization. It is intended to be used as a tool for improving an organization's cybersecurity posture and for helping organizations better understand and manage their cybersecurity risks.

**Useful Links:**

[Hướng dẫn Khởi động Nhanh NIST](https://csrc.nist.gov/Projects/cybersecurity-framework/nist-cybersecurity-framework-a-quick-start-guide)

[Khung cải thiện an ninh mạng cho hạ tầng trọng yếu](https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.04162018.pdf)

[Ứng phó với rò rỉ dữ liệu: Hướng dẫn cho doanh nghiệp](https://www.ftc.gov/business-guidance/resources/data-breach-response-guide-business)

[Sự kiện và Thuyết trình của NIST](https://www.nist.gov/cyberframework/events-and-presentations)

[Twitter - @NISTcyber](https://www.twitter.com/NISTcyber)

![image](https://user-images.githubusercontent.com/100603074/210655795-f809707f-fb3e-4df9-b07d-c4fa0392f020.png)

*Image used from https://www.dell.com/en-us/blog/strengthen-security-of-your-data-center-with-the-nist-cybersecurity-framework/*

### [🔙](#tool-list)Kế hoạch Ứng phó Sự cố

An incident response plan is a set of procedures that a company puts in place to manage and mitigate the impact of a security incident, such as a data breach or a cyber attack.
**Lưu ý:** Kế hoạch ứng phó sự cố (IR plan) là tài liệu quan trọng vạch ra các bước, vai trò, trách nhiệm và quy trình cần thực hiện khi một sự cố bảo mật xảy ra.

The theory behind an **incident response plan** is that it helps a company to be prepared for and respond effectively to a security incident, which can minimize the damage and reduce the chances of it happening again in the future.

There are several reasons why businesses need an **incident response plan**:

1. **To minimize the impact of a security incident:** An **incident response plan** helps a company to identify and address the source of a security incident as quickly as possible, which can help to minimize the damage and reduce the chances of it spreading.

2. **To meet regulatory requirements:** Many industries have regulations that require companies to have an **incident response plan** in place. For example, the Payment Card Industry Data Security Standard (**PCI DSS**) requires merchants and other organizations that accept credit cards to have an **incident response plan**.

3. **To protect reputation:** A security incident can damage a company's reputation, which can lead to a loss of customers and revenue. An **incident response plan** can help a company to manage the situation and minimize the damage to its reputation.

4. **To reduce the cost of a security incident:** The cost of a security incident can be significant, including the cost of remediation, legal fees, and lost business. An **incident response plan** can help a company to minimize these costs by providing a roadmap for responding to the incident.
**Lưu ý:** Blue Team cần xây dựng, thực hành và cập nhật thường xuyên kế hoạch này.

**Useful Links:**

[National Cyber Security Centre - Tổng quan Ứng phó Sự cố](https://www.ncsc.gov.uk/collection/incident-management/incident-response)

[SANS - Mẫu Chính sách Bảo mật](https://www.sans.org/information-security-policy/)

[SANS - Sổ tay Xử lý Sự cố](https://www.sans.org/white-papers/33901/)

[FRSecure - Mẫu Kế hoạch Ứng phó Sự cố](https://frsecure.com/incident-response-plan-template/)

[Cơ quan An ninh mạng và Hạ tầng (CISA) - ỨNG PHÓ SỰ CỐ CYBER](https://www.cisa.gov/cyber-incident-response)

[FBI - Chính sách Ứng phó Sự cố](https://www.fbi.gov/file-repository/incident-response-policy.pdf/view)

![image](https://user-images.githubusercontent.com/100603074/210656422-d75791ae-797b-4135-bbd5-8b84335892ba.png)

*Image used from https://www.ncsc.gov.uk/collection/incident-management/incident-response*

### [🔙](#tool-list)Kế hoạch Ứng phó Ransomware

Ransomware is a type of malicious software that encrypts a victim's files. The attackers then demand a ransom from the victim to restore access to the files; hence the name ransomware.
**Lưu ý:** Tấn công ransomware đã trở nên rất phổ biến và gây thiệt hại nặng nề, do đó việc có một kế hoạch ứng phó chuyên biệt là cần thiết.

The theory behind a ransomware response plan is that it helps a company to be prepared for and respond effectively to a ransomware attack, which can minimize the impact of the attack and reduce the chances of it happening again in the future.

There are several reasons why businesses need a **ransomware response plan**:

1. **To minimize the impact of a ransomware attack:** A **ransomware response plan** helps a company to identify and address a ransomware attack as quickly as possible, which can help to minimize the damage and reduce the chances of the ransomware spreading to other systems.

2. **To protect against data loss:** Ransomware attacks can result in the loss of important data, which can be costly and disruptive for a business. A **ransomware response plan** can help a company to recover from an attack and avoid data loss.

3. **To protect reputation:** A ransomware attack can damage a company's reputation, which can lead to a loss of customers and revenue. A **ransomware response plan** can help a company to manage the situation and minimize the damage to its reputation.

4. **To reduce the cost of a ransomware attack:** The cost of a ransomware attack can be significant, including the cost of remediation, legal fees, and lost business. A **ransomware response plan** can help a company to minimize these costs by providing a roadmap for responding to the attack.
**Lưu ý:** Kế hoạch này bổ sung cho kế hoạch IR chung, tập trung vào các bước đặc thù của tấn công ransomware (ví dụ: cách ly hệ thống, sao lưu, liên hệ pháp lý, thông báo...).

**Useful Links:**

[National Cyber Security Centre - Giảm thiểu tấn công malware và ransomware](https://www.ncsc.gov.uk/guidance/mitigating-malware-and-ransomware-attacks)

[NIST - Bảo vệ và Ứng phó Ransomware](https://csrc.nist.gov/Projects/ransomware-protection-and-response)

[Cơ quan An ninh mạng và Hạ tầng (CISA) - Hướng dẫn Ransomware](https://www.cisa.gov/stopransomware/ransomware-guide)

[Microsoft Security - Ứng phó Ransomware](https://www.microsoft.com/en-us/security/blog/2019/12/16/ransomware-response-to-pay-or-not-to-pay/)

[Blog - Xây dựng Kế hoạch Ứng phó Ransomware](https://www.msp360.com/resources/blog/designing-a-ransomware-response-plan/)

![image](https://user-images.githubusercontent.com/100603074/210655863-d4044516-022a-4f6b-afaa-cf375c1f01b4.png)

*Image used from https://csrc.nist.gov/Projects/ransomware-protection-and-response*

### [🔙](#tool-list)Hướng dẫn Tham khảo Ứng phó Sự cố

This is a “first aid” style of guidance for cybersecurity to help you prepare for a crisis and limit the potential damage in a crisis.
**Lưu ý:** Tài liệu này là một bản tóm tắt hướng dẫn nhanh, giống như "sổ tay cấp cứu" cho sự cố bảo mật lớn.

This includes tips and guidance for technical, operational, legal, and communications aspects of a major cybersecurity incident.

**Key Takeaways**

- **Preparation pays off** – Preparing for a major incident can reduce damage to the organization, as well as reduce incident cost and management difficulty.
- **Operationalize your incident management processes** – Managing major cybersecurity incidents must be part of standard business risk management processes.
- **Coordination is critical** – Effective cybersecurity incident management requires collaboration and coordination of technical, operations, communications, legal, and governance functions.
- **Stay calm and do no harm in an incident** – Overreacting can be as damaging as underreacting.
**Lưu ý:** Các điểm cốt lõi này nhấn mạnh tầm quan trọng của việc chuẩn bị, phối hợp giữa các bộ phận và sự bình tĩnh khi xử lý sự cố.

You can read the paper [tại đây](https://info.microsoft.com/rs/157-GQE-382/images/EN-US-CNTNT-emergency-doc-digital.pdf).

![image](https://user-images.githubusercontent.com/100603074/223865803-a026ad87-00dd-4458-bf17-416a091566dd.png)

*Image used from https://info.microsoft.com/rs/157-GQE-382/images/EN-US-CNTNT-emergency-doc-digital.pdf*

### [🔙](#tool-list)[**Awesome Incident Response**](https://github.com/meirwah/awesome-incident-response)

A curated list of tools and resources for **security incident response**, aimed to help security analysts and [DFIR](https://www.acronymfinder.com/Digital-Forensics%2c-Incident-Response-%28DFIR%29.html) teams.
**Lưu ý:** "Awesome" trong tên các repo GitHub thường có nghĩa là danh sách tuyển chọn các tài nguyên tốt về một chủ đề cụ thể. Repo này là danh sách tổng hợp nhiều công cụ và tài liệu khác nhau liên quan đến ứng phó sự cố và pháp y kỹ thuật số (DFIR).

This is a great resource full of links for different aspects of **incident response**, including:

- Adversary Emulation
- All-In-One Tools
- Books
- Communities
- Disk Image Creation Tools
**Lưu ý:** Danh sách phân loại các công cụ và tài nguyên theo các lĩnh vực khác nhau của IR/DFIR. Rất hữu ích để tìm kiếm tool cho một nhiệm vụ cụ thể.

Visit the resource [tại đây](https://github.com/meirwah/awesome-incident-response).

![image](https://user-images.githubusercontent.com/100603074/223865479-b54a2f98-0c2c-4bf1-8072-58ea7bfe4fb0.png)

*Image used from https://github.com/meirwah/awesome-incident-response*

**Phát hiện và Phân tích Malware**
====================

*Các công cụ để phát hiện và phân tích **malware**, bao gồm phần mềm **antivirus** và công cụ phân tích pháp y.*

### [🔙](#tool-list)[**VirusTotal**](https://www.virustotal.com/gui/home/search)

**VirusTotal** is a website and cloud-based tool that analyzes and scans files, URLs, and software for viruses, worms, and other types of **malware**.
**Lưu ý:** VirusTotal là một dịch vụ trực tuyến rất nổi tiếng để kiểm tra một file hoặc URL có phải là độc hại không, bằng cách chạy nó qua nhiều bộ máy AV khác nhau và cung cấp kết quả.

When a file, URL, or software is submitted to **VirusTotal**, the tool uses various **antivirus** engines and other tools to scan and analyze it for **malware**. It then provides a report with the results of the analysis, which can help security professionals and blue teams identify and respond to potential threats.

**VirusTotal** can also be used to check the reputation of a file or URL, and to monitor for malicious activity on a network.
**Lưu ý:** Ngoài quét, VirusTotal còn tổng hợp thông tin từ nhiều nguồn (chữ ký AV, sandbox analysis, cộng đồng) để đưa ra đánh giá rủi ro và các thông tin liên quan (giao tiếp C2, dropped file,...). Blue Team dùng nó để phân loại sample, tìm kiếm IoC.

Visit [https://www.virustotal.com/gui/home/search](https://www.virustotal.com/gui/home/search)

**Usage:**

```bash
# Các tài liệu mới được tạo có nhúng macro, được ít nhất 5 AV phát hiện
(type:doc OR type: docx) tag:macros p:5+ generated:30d+

# Tệp Excel đi kèm với script powershell và được tải lên VT trong 10 ngày qua
(type:xls OR type:xlsx) tag:powershell fs:10d+

# Payload exploit kiểu Follina
entity:file magic:"HTML document text" tag:powershell have:itw_url

# Các URL liên quan đến domain/subdomain cha cụ thể với một header nhất định trong phản hồi
entity:url header_value:"Apache/2.4.41 (Ubuntu)" parent_domain:domain.org

# Các URL đáng ngờ với title HTML cụ thể
entity:url ( title:"XY Company" or title:"X.Y. Company" or title:"XYCompany" ) p:5+
```
**Lưu ý:** Các ví dụ này là cú pháp tìm kiếm nâng cao trong **VirusTotal Intelligence** (dịch vụ trả phí) hoặc VirusTotal Graph. Chúng cho phép Blue Team tìm kiếm các file hoặc URL phù hợp với các tiêu chí phức tạp (loại file, tag, số lượng phát hiện, ngày tải lên, nội dung, header response...), rất mạnh cho threat hunting và phân tích các chiến dịch tấn công cụ thể.

Full documentation can be found [tại đây](https://support.virustotal.com/hc/en-us/categories/360000162878-Documentation).

[VT INTELLIGENCE CHEAT SHEET](https://storage.googleapis.com/vtpublic/reports/VTI%20Cheatsheet.pdf)

![image](https://user-images.githubusercontent.com/100603074/210655958-9a39783e-637e-46a3-a80c-4c64b389de60.png)

*Image used from https://www.virustotal.com/gui/home/search*

### [🔙](#tool-list)[**IDA**](https://hex-rays.com/ida-free/)

**IDA** (Interactive Disassembler) is a powerful tool used to reverse engineer and analyze compiled and executable code.

It can be used to examine the inner workings of software, including malware, and to understand how it functions. **IDA** allows users to disassemble code, decompile it into a higher-level programming language, and view and edit the resulting source code. This can be useful for identifying vulnerabilities, analyzing malware, and understanding how a program works.

**IDA** can also be used to generate graphs and charts that visualize the structure and flow of code, which can make it easier to understand and analyze.
**Lưu ý:** IDA là một trong những trình dịch ngược và gỡ lỗi mạnh nhất và đắt tiền nhất. Các nhà phân tích malware (Blue Team chuyên sâu) sử dụng nó để hiểu cách hoạt động của malware ở mức mã máy/mã assembly và mã giả (pseudocode).

**Install:**

Download IDA from [tại đây](https://hex-rays.com/ida-free/#download).
**Lưu ý:** Có phiên bản miễn phí (IDA Free) nhưng bị giới hạn tính năng và kiến trúc hỗ trợ so với phiên bản thương mại.

**Usage:**

[**IDA** Practical Cheatsheet](https://github.com/AdamTaguirov/IDA-practical-cheatsheet)

[**IDAPython** cheatsheet](https://gist.github.com/icecr4ck/7a7af3277787c794c66965517199fc9c)
**Lưu ý:** IDAPython cho phép script hóa các tác vụ trong IDA.

[**IDA Pro** Cheatsheet](https://hex-rays.com/products/ida/support/freefiles/IDA_Pro_Shortcuts.pdf)

![image](https://user-images.githubusercontent.com/100603074/210655977-e52a66eb-7698-4769-b002-a9d6f1503b85.png)

*Image used from https://www.newton.com.tw/wiki/IDA%20Pro*

### [🔙](#tool-list)[**Ghidra**](https://ghidra-sre.org/)

**Ghidra** is a free, open-source software reverse engineering tool developed by the **National Security Agency (NSA)**. It is used to analyze compiled and executable code, including malware.
**Lưu ý:** Ghidra là một giải pháp thay thế mã nguồn mở miễn phí rất mạnh mẽ cho IDA, do NSA phát triển và phát hành công khai.

**Ghidra** allows users to disassemble code, decompile it into a higher-level programming language, and view and edit the resulting source code. This can be useful for identifying vulnerabilities, analyzing malware, and understanding how a program works.

**Ghidra** also includes a range of features and tools that support SRE tasks, such as debugging, code graphing, and data visualization. **Ghidra** is written in Java and is available for Windows, MacOS, and Linux.
**Lưu ý:** Ghidra hỗ trợ nhiều kiến trúc xử lý và có một môi trường đồ họa toàn diện cho phép phân tích binary (ngược dịch, gỡ lỗi, vẽ đồ thị luồng điều khiển). Nó rất phổ biến với các nhà phân tích malware do tính miễn phí và khả năng.

**Install:**

1. Download the latest release from [tại đây](https://github.com/NationalSecurityAgency/ghidra/releases).
2. Extract the zip
**Lưu ý:** Chỉ cần tải tệp zip và giải nén, Ghidra chạy bằng Java nên không cần cài đặt phức tạp (ngoài JRE).

Full installation and error fix information can be found [tại đây](https://ghidra-sre.org/InstallationGuide.html#Install).

**Usage:**

1. Navigate to the unzipped folder

```bash
# Windows
ghidraRun.bat

# Linux
./ghidraRun
```
**Lưu ý:** Chạy script để khởi động Ghidra trên các hệ điều hành.

If **Ghidra** failed to launch, see the [Troubleshooting](https://ghidra-sre.org/InstallationGuide.html#Troubleshooting) link.

![image](https://user-images.githubusercontent.com/100603074/210656000-9b31d5fc-7b95-447e-94ed-94aef602de46.png)

*Image used from https://www.malwaretech.com/2019/03/video-first-look-at-ghidra-nsa-reverse-engineering-tool.html*

### [🔙](#tool-list)[**decode-vbe**](https://github.com/DidierStevens/DidierStevensSuite/blob/master/decode-vbe.py)

Script Encoding was introduced by **Microsoft** (long ago) to prevent people from being able to read, understand and alter **VBScript** files.

Encoded scripts are unreadable but still able to execute, making it a popular mechanism with threat actors looking to hide their malicious code, IOCs, hardcoded **C2** domains etc whilst still being able to achieve execution.
**Lưu ý:** VBScript Encoding (dạng `.vbe` file) là một kỹ thuật cũ nhưng vẫn đôi khi được dùng để che giấu mã nguồn VBScript độc hại. Các file `.vbe` khó đọc trực tiếp.

The **decode-vbe script** can be used to convert encoded **VBE files** back to plaintext for analysis.
**Lưu ý:** Script này là một công cụ nhỏ nhưng rất hữu ích cho các nhà phân tích **malware** khi gặp các mẫu `.vbe` được mã hóa, cho phép họ lấy được mã nguồn gốc để hiểu chức năng độc hại.

Nice blog about VBE files [tại đây](https://bromiley.medium.com/malware-monday-vbscript-and-vbe-files-292252c1a16).

**Install:**

```bash
git clone https://github.com/DidierStevens/DidierStevensSuite/
cd DidierStevensSuite
```
**Lưu ý:** Clone repository chứa bộ script của Didier Stevens, **decode-vbe.py** là một phần trong bộ này.

**Usage:**

```bash
# Decode chuỗi ký tự
decode-vbe.py "##@~^DgAAAA==\ko$K6,JCV^GJqAQAAA==^#~@"

# Decode hệ thập lục phân (prefix #h#)
decode-vbe.py #h#23407E5E4467414141413D3D5C6B6F244B362C4A437F565E474A7141514141413D3D5E237E40

# Decode base64 (prefix #b#)
decode-vbe.py #b#I0B+XkRnQUFBQT09XGtvJEs2LEpDf1ZeR0pxQVFBQUE9PV4jfkA=
```
**Lưu ý:** Ví dụ cách chạy script **decode-vbe.py** với các loại input khác nhau: chuỗi VBE mã hóa trực tiếp, chuỗi hex, chuỗi base64. Script tự nhận dạng định dạng nếu có prefix tương ứng.

### [🔙](#tool-list)[**pafish**](https://github.com/a0rtega/pafish)

**Pafish** is a testing tool that uses different techniques to detect virtual machines and malware analysis environments in the same way that **malware families** do.
**Lưu ý:** Nhiều loại malware hiện đại có cơ chế kiểm tra môi trường chạy để phát hiện xem chúng đang ở trong sandbox, máy ảo, hoặc bị gỡ lỗi. Nếu phát hiện, malware có thể không thực thi chức năng độc hại để tránh bị phân tích.

The project is free and open source; the code of all the anti-analysis techniques is publicly available. **Pafish executables** for Windows (**x86** 32-bit and 64-bit) can be downloaded from the [releases page](https://github.com/a0rtega/pafish/releases).

**Install (Build):**

**Pafish** is written in C and can be built with **Mingw-w64** and make.
**Lưu ý:** Yêu cầu các công cụ build C.

The wiki page "[Cách Build](https://github.com/a0rtega/pafish/wiki/How-to-build)" contains detailed instructions.

**Usage:**

```bash
pafish.exe
```
**Lưu ý:** Chạy tệp thực thi `pafish.exe`. Nó sẽ tự động thực hiện các kiểm tra và báo cáo xem có phát hiện ra môi trường phân tích hay không. Blue Team có thể sử dụng công cụ này để kiểm tra xem sandbox hoặc máy phân tích của mình có bị phát hiện bởi các kỹ thuật **anti-analysis** phổ biến không, từ đó cải thiện môi trường.

![image](https://user-images.githubusercontent.com/100603074/218870623-4c149ec7-2002-42ea-9c24-0d35f562bb8c.png)

*Image used from https://github.com/a0rtega/pafish*

### [🔙](#tool-list)[**lookyloo**](https://github.com/Lookyloo/lookyloo)

**Lookyloo** is a web interface that captures a webpage and then displays a tree of the domains, that call each other.
**Lưu ý:** Lookyloo là một công cụ phân tích hành vi trang web (web page behavior analysis). Nó truy cập một URL, ghi lại quá trình tải trang, các kết nối đến domain khác, các redirect, và vẽ sơ đồ mối quan hệ giữa các domain được tải.

Use **Lookyloo** to map the journey a website page takes - from entering the initial URL address to the various redirects to third-party affiliations.
**Lưu ý:** Rất hữu ích cho Blue Team để phân tích các URL đáng ngờ, email phishing hoặc các trang web quảng cáo độc hại (malvertising) để hiểu luồng redirect, các domain trung gian và domain đích cuối cùng, cũng như các tài nguyên khác được tải về.

**Install:**

```bash
git clone https://github.com/Lookyloo/lookyloo.git
cd lookyloo
poetry install
echo LOOKYLOO_HOME="'`pwd`'" > .env
```
**Lưu ý:** Tải mã nguồn và sử dụng **poetry** (trình quản lý dependency Python) để cài đặt. Thiết lập biến môi trường `LOOKYLOO_HOME`.

Full installation instructions can be found [tại đây](https://www.lookyloo.eu/docs/main/install-lookyloo.html).

**Usage:**

Once installed and running, **lookyloo** can be operated via the web interface hosted locally.
**Lưu ý:** Truy cập giao diện web sau khi server đã chạy để gửi các URL cần phân tích.

![image](https://user-images.githubusercontent.com/100603074/218870701-24d0b7c1-50d9-4b7d-9b9d-b76c98b4e10f.png)

*Image used from https://www.lookyloo.eu/*

### [🔙](#tool-list)[**YARA**](https://github.com/virustotal/yara)

**YARA** is a tool aimed at (but not limited to) helping **malware researchers** to identify and classify malware samples. With **YARA** you can create descriptions of malware families (or whatever you want to describe) based on textual or binary patterns.
**Lưu ý:** YARA là một **công cụ** khung (framework) để tạo các luật dựa trên pattern để tìm kiếm các file hoặc mẫu dữ liệu phù hợp. Cú pháp luật YARA bao gồm các chuỗi text hoặc binary và một biểu thức logic để xác định khi nào luật được coi là khớp.

Each description, a.k.a rule, consists of a set of strings and a boolean expression which determine its logic.
**Lưu ý:** Các nhà phân tích malware và Blue Team sử dụng luật YARA để phát hiện các biến thể malware mới, tìm kiếm các file chứa IoC đã biết, hoặc phân loại các mẫu độc hại.

**Install:**

```bash
tar -zxf yara-4.2.0.tar.gz
cd yara-4.2.0
./bootstrap.sh
sudo apt-get install automake libtool make gcc pkg-config
git clone https://github.com/VirusTotal/yara
cd yara
./bootstrap.sh
./configure
make
sudo make install
```
**Lưu ý:** Các lệnh để cài đặt YARA từ mã nguồn. Nó yêu cầu các công cụ build C và các thư viện dependency (`automake`, `libtool`...). Khuyến khích cài đặt từ trình quản lý gói của hệ điều hành (apt, yum, brew...) nếu có sẵn.

Full installation instructions can be found [tại đây](https://yara.readthedocs.io/en/stable/gettingstarted.html#compiling-and-installing-yara).

**Usage:**

```bash
# Apply rule in /foo/bar/rules to all files in the current directory
yara /foo/bar/rules .

# Scan all files in the /foo directory and its subdirectories:
yara /foo/bar/rules -r /foo
```
**Lưu ý:** Sử dụng **command line utility yara**. `yara` cần đường dẫn đến file luật YARA và đường dẫn đến file hoặc thư mục cần quét. `-r` bật quét đệ quy. Output cho biết những file nào khớp với luật nào. Blue Team dùng để quét file trên endpoint, trên server file hoặc trong sandbox để phát hiện malware.

Nice **YARA** cheatsheet [tại đây](https://github.com/mattnotmax/DFIR-notes/blob/master/cheatsheet_yara.md).

![image](https://user-images.githubusercontent.com/100603074/218871209-da726de1-1563-40b4-857c-3234f7415fdb.png)

*Image used from https://virustotal.github.io/yara/*

### [🔙](#tool-list)[**Cuckoo Sandbox**](https://cuckoosandbox.org/)

**Cuckoo** is an open source automated **malware analysis system**.
**Lưu ý:** Cuckoo Sandbox là một hệ thống sandbox tự động (sandbox automated analysis) để chạy malware một cách an toàn và quan sát hành vi của nó. Rất hữu ích cho các nhà phân tích malware và Blue Team.

It’s used to automatically run and analyze files and collect comprehensive analysis results that outline what the malware does while running inside an isolated operating system.
**Lưu ý:** Sandbox tạo một môi trường an toàn (máy ảo hoặc container) để cho phép malware thực thi mà không gây hại cho hệ thống thật.

It can retrieve the following type of results:

- Traces of calls performed by all processes spawned by the malware.
- Files being created, deleted and downloaded by the malware during its execution.
- Memory dumps of the malware processes.
- Network traffic trace in PCAP format.
- Screenshots taken during the execution of the malware.
- Full memory dumps of the machines.
**Lưu ý:** Cuckoo tự động thu thập rất nhiều loại dữ liệu chi tiết về hành vi của malware: hoạt động của tiến trình, thay đổi file, kết nối mạng, snapshot bộ nhớ... Kết quả này giúp nhà phân tích hiểu sâu về chức năng của malware.

**Install:**

For installation follow the docs [tại đây](https://cuckoo.readthedocs.io/en/latest/installation/).

**Usage:**

For usage follow the docs [tại đây](https://cuckoo.readthedocs.io/en/latest/usage/).

### [🔙](#tool-list)[**radare2**](https://github.com/radareorg/radare2)

**Radare2** provides a set of libraries, tools and plugins to ease reverse engineering tasks.

**r2** is a featureful low-level command-line tool with support for scripting. **r2** can edit files on local hard drives, view kernel memory, and debug programs locally or via a remote gdb server. **r2**'s wide architecture support allows you to analyze, emulate, debug, modify, and disassemble any binary.
**Lưu ý:** Radare2 (r2) là một framework dịch ngược và phân tích binary mã nguồn mở. Nó hoạt động chủ yếu thông qua giao diện dòng lệnh, rất linh hoạt và có nhiều chức năng (dịch ngược, debug, phân tích binary, giả lập...). Là giải pháp thay thế cho IDA hoặc Ghidra (đặc biệt là khi thích làm việc trên command line).

**Install:**

```bash
git clone https://github.com/radareorg/radare2
radare2/sys/install.sh
```
**Lưu ý:** Tải mã nguồn và chạy script cài đặt.

**Usage:**

```bash
$ r2 /bin/ls   # mở binary ở chế độ chỉ đọc
> aaa          # giống như r2 -A, phân tích binary
> afl          # liệt kê tất cả các hàm (thử aflt, aflm)
> px 32        # in hexdump 32 byte của khối hiện tại
> s sym.main   # di chuyển đến offset được cho (bằng tên flag, số, ..)
> f~foo        # lọc flags với ~grep (giống như |grep)
> iS;is        # liệt kê các section và symbols (giống như rabin2 -Ss)
> pdf; agf     # in hàm và hiển thị biểu đồ luồng điều khiển dạng ascii-art
> oo+;w hello  # mở lại ở chế độ rw và ghi một chuỗi tại offset hiện tại
> ?*~...       # bộ lọc tương tác tất cả các thông báo trợ giúp lệnh
> q            # thoát
```
**Lưu ý:** Đây là các lệnh phổ biến trong console **r2**. **Blue Team** dùng để phân tích sâu mã binary, hiểu cấu trúc file, logic của malware.

Great usage book [tại đây](https://book.rada.re/).

![image](https://user-images.githubusercontent.com/100603074/218871325-90800880-ee58-4a61-9372-fa9cb09f6bf3.png)

*Image used from https://github.com/radareorg/radare2*

### [🔙](#tool-list)[**dnSpy**](https://github.com/dnSpy/dnSpy)

**dnSpy** is a debugger and .NET assembly editor. You can use it to edit and debug assemblies.
**Lưu ý:** dnSpy là công cụ chuyên biệt để làm việc với các binary/assembly của .NET Framework và .NET Core.

Main features:

- Debug .NET and Unity assemblies
- Edit .NET and Unity assemblies
**Lưu ý:** Malware viết bằng C# hoặc các ngôn ngữ .NET khác rất phổ biến. **dnSpy** cho phép Blue Team gỡ lỗi (debug) trực tiếp các assembly .NET, dịch ngược chúng thành mã nguồn C# và thậm chí chỉnh sửa rồi lưu lại assembly đã thay đổi. Cực kỳ quan trọng khi phân tích malware .NET.

**Install (Build):**

```bash
git clone --recursive https://github.com/dnSpy/dnSpy.git
cd dnSpy
./build.ps1 -NoMsbuild
```
**Lưu ý:** Clone mã nguồn (bao gồm submodule) và chạy script PowerShell để build.

**Usage:**

```bash
dnSpy.exe
```
**Lưu ý:** Chạy tệp thực thi **dnSpy**. Nó có giao diện đồ họa.

Nice tutorial page [tại đây](https://7d2dsdx.github.io/Tutorials/index.html?StartingdnSpy.html).

![image](https://user-images.githubusercontent.com/100603074/218871411-7eb20cb7-f2e8-4d29-98a9-d5820a138c8e.png)

*Image used from https://7d2dsdx.github.io/Tutorials/index.html?StartingdnSpy.html*

### [🔙](#tool-list)[**malware-traffic-analysis.net**](https://www.malware-traffic-analysis.net/)

This is a site with over 2,200 blog entries about malicious network traffic. Almost every post on the site has pcap files or malware samples (or both).
**Lưu ý:** Đây là một nguồn tài nguyên trực tuyến chứa rất nhiều bài viết phân tích về lưu lượng mạng liên quan đến malware, đi kèm với các file PCAP (packet capture) và mẫu malware.

The site also contains a number of traffic analysis exercises, including technical blog posts outlining techniques being used by threat actors.
**Lưu ý:** Nguồn tài nguyên này cực kỳ hữu ích cho Blue Team và những người làm threat hunting hoặc network forensics để luyện tập kỹ năng phân tích lưu lượng mạng thực tế liên quan đến các loại malware và TTP khác nhau.

**Usage:**

Visit [https://www.malware-traffic-analysis.net/](https://www.malware-traffic-analysis.net/).

![image](https://user-images.githubusercontent.com/100603074/218871486-f782e3f1-fcea-4e68-a99b-235146490b84.png)

*Image used from https://www.malware-traffic-analysis.net/*

**Phục hồi Dữ liệu**
====================

*Các công cụ để phục hồi dữ liệu từ hệ thống và thiết bị bị hỏng hoặc bị lỗi.*

### [🔙](#tool-list)[**Recuva**](https://www.ccleaner.com/recuva)

**Recuva** is a data recovery tool that can be used to recover deleted files from your computer.
**Lưu ý:** Recuva là công cụ phổ biến và dễ sử dụng để phục hồi file đã xóa (do vô tình, định dạng hoặc bởi malware xóa).

It is often used to recover deleted files that may contain valuable information, such as deleted logs or documents that could be used to investigate a security incident.

**Recuva** can recover files from hard drives, USB drives, and memory cards, and it is available for Windows and Mac operating systems.
**Lưu ý:** Blue Team có thể dùng Recuva trong quá trình điều tra để tìm kiếm các file bằng chứng quan trọng có thể đã bị xóa bởi attacker hoặc do sự cố.

**Install:**

You can download the tool from [tại đây](https://www.ccleaner.com/recuva).

**Usage:**

Nice step by step [guide](https://toolbox.iskysoft.com/data-recovery-tips/recuva-windows-10.html).

![image](https://user-images.githubusercontent.com/100603074/210668891-58312f55-d4d0-4f77-9cd6-f716bbdb5b44.png)

*Image used from https://www.softpedia.com/blog/recuva-explained-usage-video-and-download-503681.shtml*

### [🔙](#tool-list)[**Extundelete**](https://extundelete.sourceforge.net/)

**Extundelete** is a utility that can be used to recover deleted files from an **ext3** or **ext4** file system.
**Lưu ý:** Ext3/Ext4 là các định dạng file system phổ biến trên Linux. **Extundelete** chuyên biệt cho việc phục hồi file đã xóa trên các phân vùng Linux sử dụng các định dạng này.

It works by searching the file system for blocks of data that used to belong to a file, and then attempting to recreate the file using those blocks of data. It is often used to recover important files that have been accidentally or maliciously deleted.

**Install:**

You can download the tool from [tại đây](https://sourceforge.net/project/platformdownload.php?group_id=260221).

**Usage:**

```bash
# In thông tin về filesystem từ superblock.
--superblock

# Cố gắng khôi phục tệp đã bị xóa tại đường dẫn được cho, gọi là "--restore-file dirname/filename".
--restore-file path/to/deleted/file

# Khôi phục tất cả các tệp có thể phục hồi đến tên của chúng trước khi xóa, nếu có thể. Các tệp khác được khôi phục thành tên như "file.NNNN".
--restore-all
```
**Lưu ý:** **Extundelete** là công cụ dòng lệnh chạy trên Linux. Nó truy cập trực tiếp vào cấu trúc của file system (thường yêu cầu mount read-only hoặc unmount phân vùng cần phục hồi để tránh ghi đè). Cú pháp `--restore-file` và `--restore-all` là các chế độ phục hồi phổ biến.

Full usage information can be found [tại đây](https://extundelete.sourceforge.net/options.html).

![image](https://user-images.githubusercontent.com/100603074/210669234-0d2d4920-7856-4731-b81c-3d7132f752ad.png)

*Image used from https://theevilbit.blogspot.com/2013/01/backtrack-forensics-ext34-file-recovery.html*

### [🔙](#tool-list)[**TestDisk**](https://www.cgsecurity.org/wiki/TestDisk_Download)

**TestDisk** is a free and open-source data recovery software tool that is designed to help recover lost partitions and make non-booting disks bootable again. It is useful for both **computer forensics and data recovery**.

It can be used to recover data that has been lost due to a variety of reasons, such as accidental deletion, formatting, or corruption of the partition table.

**TestDisk** can also be used to repair damaged boot sectors, recover deleted partitions, and recover lost files. It supports a wide range of file systems, including **FAT, NTFS**, and **ext2/3/4**, and can be used to recover data from disks that are damaged or formatted with a different file system than the one they were originally created with.
**Lưu ý:** **TestDisk** mạnh mẽ trong việc sửa chữa cấu trúc ổ đĩa và phục hồi các phân vùng bị mất hoặc bị hỏng. Nó hỗ trợ nhiều định dạng file system và là công cụ hữu ích khi hệ thống không khởi động được hoặc các phân vùng không thể truy cập bình thường. PhotoRec (thường đi kèm TestDisk) tập trung vào phục hồi file bị xóa bất kể cấu trúc file system.

**Install:**

You can download the tool from [tại đây](https://www.cgsecurity.org/wiki/TestDisk_Download).

**Usage:**

Full usage examples [tại đây](https://www.cgsecurity.org/wiki/Data_Recovery_Examples).

[Hướng dẫn từng bước TestDisk](https://www.cgsecurity.org/wiki/TestDisk_Step_By_Step)

[Tài liệu TestDisk PDF - 60 Trang](https://www.cgsecurity.org/testdisk.pdf)

![image](https://user-images.githubusercontent.com/100603074/210668956-4ed75998-bd6d-48cf-a2e7-dfa75656eece.png)

*Image used from https://www.cgsecurity.org/wiki/*

**Pháp y Kỹ thuật số**
====================

*Các công cụ để tiến hành điều tra pháp y trên các thiết bị và hệ thống kỹ thuật số, bao gồm các công cụ để thu thập và phân tích bằng chứng.*

### [🔙](#tool-list)[**SANS SIFT**](https://www.sans.org/tools/sift-workstation/)

**SANS SIFT (SANS Investigative Forensic Toolkit)** is a powerful **toolkit** for **forensic analysis** and **incident response**.
**Lưu ý:** SIFT là một bản phân phối Linux (dưới dạng máy ảo hoặc cài đặt trên Ubuntu/Debian) được cài sẵn rất nhiều công cụ pháp y kỹ thuật số (DFIR) mã nguồn mở và một số công cụ khác. Rất tiện lợi cho các nhà điều tra pháp y và Blue Team.

It is a collection of open source and commercial tools that can be used to perform **forensic analysis** on a wide range of systems, including Windows, Linux, and Mac OS X. The **SANS SIFT** kit is designed to be run on a **forensic workstation**, which is a specialized computer that is used to perform forensic analysis on digital evidence.

The **SANS SIFT** kit is particularly useful for blue teamers, as it provides a wide range of tools and resources that can be used to investigate incidents, respond to threats, and perform **forensic analysis** on compromised systems.
**Lưu ý:** Blue Team dùng SIFT workstation để phân tích ảnh đĩa (disk image) của các máy bị sự cố mà không ảnh hưởng đến bằng chứng gốc.

**Install:**

1. Visit [https://www.sans.org/tools/sift-workstation/](https://www.sans.org/tools/sift-workstation/).

2. Click the '**Login to Download**' button and input (or create) your SANS Portal account credentials to download the **virtual machine**.

3. Once you have booted the **virtual machine**, use the credentials below to gain access.

```
Login = sansforensics
Password = forensics
```
**Lưu ý:** Hướng dẫn tải và truy cập máy ảo SIFT.

**Note:** *Use to elevate privileges to root while mounting disk images.*
**Lưu ý:** Cần dùng tài khoản mặc định và `sudo` hoặc `su` để có quyền root cho các tác vụ DFIR cấp thấp như mount ảnh đĩa.

Additional install options [tại đây](https://www.sans.org/tools/sift-workstation/).

**Usage:**

```bash
# Registry Parsing - Regripper
rip.pl -r <HIVEFILE> -f <HIVETYPE>

# Recover deleted registry keys
deleted.pl <HIVEFILE>

# Mount E01 Images
ewfmount image.E01 mountpoint
mount -o

# Stream Extraction
bulk_extractor <options> -o output_dir
```
**Lưu ý:** Các ví dụ sử dụng một số công cụ có sẵn trong SIFT:
`rip.pl` (Regripper) là công cụ phân tích file registry hive của Windows.
`deleted.pl` phục hồi các khóa registry bị xóa.
`ewfmount` dùng để mount ảnh đĩa pháp y định dạng E01 (Expert Witness Format).
`bulk_extractor` là công cụ quét nhanh các file trên ổ đĩa hoặc ảnh đĩa để tìm các loại thông tin cụ thể (email address, URL, chuỗi ký tự...).

Full usage guide [tại đây](https://www.sans.org/posters/sift-cheat-sheet/).

![image](https://user-images.githubusercontent.com/100603074/210668984-bdec731b-ce80-4c3b-9696-9431dd77f9b0.png)

*Image used from https://securityboulevard.com/2020/08/how-to-install-sift-workstation-and-remnux-on-the-same-system-for-forensics-and-malware-analysis/*

### [🔙](#tool-list)[**The Sleuth Kit**](https://sleuthkit.org/sleuthkit/)

**The Sleuth Kit** is a collection of command line tools that can be used to analyze disk images and recover files from them.
**Lưu ý:** Đây là một bộ công cụ dòng lệnh nền tảng cho pháp y kỹ thuật số trên nhiều hệ điều hành. Các công cụ như `fsstat`, `ils`, `blkcat`, `icat` cho phép phân tích cấu trúc file system, liệt kê file, đọc nội dung inode,...

It is primarily used by **forensic investigators** to examine digital evidence after a computer has been seized or an image of a disk has been made. It can be useful because it can help understand what happened during a security incident and identify any malicious activity.

The tools in **The Sleuth Kit** can be used to extract deleted files, analyze disk partition structures, and examine the file system for evidence of tampering or unusual activity.
**Lưu ý:** Các công cụ trong Sleuth Kit cho phép phục hồi dữ liệu, phân tích các partition, hiểu cách file được lưu trữ trên đĩa và tìm dấu vết attacker.

**Install:**

Download tool from [tại đây](https://sleuthkit.org/sleuthkit/download.php).

**Usage:**

Link to [documentation](https://sleuthkit.org/sleuthkit/docs.php).

![image](https://user-images.githubusercontent.com/100603074/210669006-6dfab59d-b50e-49db-b390-b9ef27cab6fe.png)

*Image used from http://www.effecthacking.com/2016/09/the-sleuth-kit-digital-forensic-tool.html*

### [🔙](#tool-list)[**Autopsy**](https://www.autopsy.com/)

**Autopsy** is a **digital forensics platform** and graphical interface to **The Sleuth Kit** and other digital forensics tools.
**Lưu ý:** Autopsy cung cấp một giao diện người dùng đồ họa (GUI) cho The Sleuth Kit và nhiều công cụ pháp y khác, làm cho quá trình điều tra dễ tiếp cận hơn cho những người không quen thuộc với dòng lệnh.

It is used by law enforcement, military, and corporate examiners to investigate what happened on a computer. You can use it to analyze disk images and recover files, as well as to identify system and user activity.

**Autopsy** is used by "**blue teams**" (the cybersecurity professionals who defend organizations against attacks) to conduct forensic analysis and **incident response**. It can help **blue teams** understand the nature and scope of an attack, and identify any malicious activity that may have occurred on a computer or network.
**Lưu ý:** Blue Team dùng Autopsy để phân tích các ảnh đĩa từ máy tính bị sự cố (compromised endpoints), tìm kiếm bằng chứng về hành vi của attacker: file được tạo/sửa/xóa, activity registry, log sự kiện, network connection, artifact trình duyệt...

**Install:**

Download the tool from [tại đây](https://www.autopsy.com/download/).

**Usage:**

[Hướng dẫn sử dụng Autopsy](http://sleuthkit.org/autopsy/docs/user-docs/4.19.3//)

[SANS - Giới thiệu sử dụng Trình duyệt Pháp y AUTOPSY](https://www.sans.org/blog/a-step-by-step-introduction-to-using-the-autopsy-forensic-browser/)

![image](https://user-images.githubusercontent.com/100603074/210669037-449e7790-85c8-4b8c-97b9-2b46a1ea6e61.png)

*Image used from https://www.kitploit.com/2014/01/autopsy-digital-investigation-analysis.html*

**Đào tạo Nhận thức An ninh**
====================

*Các công cụ để đào tạo nhân viên và người dùng khác về cách nhận dạng và ngăn chặn các mối đe dọa bảo mật tiềm ẩn.*

### [🔙](#tool-list)[**TryHackMe**](https://tryhackme.com/dashboard)

**TryHackMe** is a platform that offers a variety of virtual machines, known as "rooms," which are designed to teach cybersecurity concepts and skills through hands-on learning.
**Lưu ý:** TryHackMe cung cấp các bài lab thực hành về an ninh mạng, bao gồm cả các phòng (room) tập trung vào kỹ năng Blue Team và Incident Response.

These rooms are interactive and gamified, allowing users to learn about topics such as web vulnerabilities, network security, and cryptography by solving challenges and completing tasks.

The platform is often used for security awareness training, as it provides a safe and controlled environment for users to practice their skills and learn about different types of cyber threats and how to defend against them.
**Lưu ý:** Là nguồn tuyệt vời để đào tạo thành viên Blue Team và nâng cao nhận thức cho nhân viên bằng cách cho họ trải nghiệm (trong môi trường an toàn) các loại tấn công và cách phát hiện/phòng vệ.

Visit [https://tryhackme.com/](https://tryhackme.com/) and create an account.

[**TryHackMe** - Hướng dẫn Bắt đầu](https://docs.tryhackme.com/docs/teaching/teaching-getting-started/)

**Useful links:**

[Đường dẫn Học tập Tiền-An ninh](https://tryhackme.com/path-action/presecurity/join)

[Giới thiệu về Đường dẫn Học tập An ninh mạng](https://tryhackme.com/path-action/introtocyber/join)

Visit the [hacktivities](https://tryhackme.com/hacktivities) tab for a full list of available rooms and modules.

![image](https://user-images.githubusercontent.com/100603074/210669062-dba079b7-a677-4b7a-ac99-6892ba894ac8.png)

*Image used from https://www.hostingadvice.com/blog/learn-cybersecurity-with-tryhackme/*

### [🔙](#tool-list)[**HackTheBox**](https://www.hackthebox.com/)

**HackTheBox** is a platform for practicing and improving your hacking skills.
**Lưu ý:** HackTheBox chủ yếu tập trung vào các bài lab tấn công (offensive security/penetration testing), nhưng việc hiểu cách thức attacker hoạt động là rất quan trọng đối với Blue Team.

It consists of a set of challenges that simulate real-world scenarios and require you to use your knowledge of various hacking techniques to solve them. These challenges are designed to test your knowledge of topics such as network security, cryptography, web security, and more.

**HackTheBox** is often used by security professionals as a way to practice and improve their skills, and it can also be a useful resource for security awareness training. By working through the challenges and learning how to solve them, individuals can gain a better understanding of how to identify and mitigate common security threats.
**Lưu ý:** Mặc dù tập trung tấn công, việc luyện tập trên HTB giúp Blue Team "nghĩ như attacker", từ đó hiểu các lỗ hổng, TTPs, và cách củng cố phòng thủ tốt hơn.

Visit [https://app.hackthebox.com/login](https://app.hackthebox.com/login) and create an account.

**Useful links:**

[Blog - Giới thiệu về Hack The Box](https://help.hackthebox.com/en/articles/5185158-introduction-to-hack-the-box)

[Blog - Học Hack với Hack The Box: Kinh thánh cho người mới bắt đầu](https://www.hackthebox.com/blog/learn-to-hack-beginners-bible)

[Blog - Giới thiệu về Starting Point](https://help.hackthebox.com/en/articles/6007919-introduction-to-starting-point)

![image](https://user-images.githubusercontent.com/100603074/210669087-d00d76d1-300f-48c9-8f7f-4b9b5157626e.png)

*Image used from https://www.hackthebox.com/login*

### [🔙](#tool-list)[**CyberDefenders**](https://cyberdefenders.org/)

**CyberDefenders** is a dedicated platform designed for **blue team professionals** to enhance their **cyber security skills**.
**Lưu ý:** Nền tảng này tập trung chuyên biệt vào các kỹ năng phòng thủ cho Blue Team.

The platform provides real-world **blue team labs** that cover a broad range of disciplines. Participants are encouraged to apply their knowledge in areas such as **incident response, digital forensics, and threat hunting** to navigate through these scenarios.

The goal is to offer a practical learning environment that mirrors the complexities that defenders encounter in Security Operations Centers.
**Lưu ý:** Cung cấp các bài lab thực hành giả lập các tình huống thực tế liên quan đến ứng phó sự cố, pháp y, và threat hunting.

Visit [https://cyberdefenders.org/](https://cyberdefenders.org/) and create an account.

**Useful links:**

[Các Bài Lab Blue Team](https://cyberdefenders.org/blue-team-labs/)

[Chứng nhận Certified CyberDefender](https://cyberdefenders.org/blue-team-training/courses/certified-cyberdefender-certification/)

![image](https://github.com/ahmedkhalidali/BlueTeam-Tools/assets/30199198/fe2ef3c9-d8a9-4a82-91c8-d93487df3afb)

### [🔙](#tool-list)[**PhishMe**](https://cofense.com/product-services/phishme/)

**PhishMe** is a company that provides **security awareness training** to help organizations educate their employees about how to identify and prevent phishing attacks.
**Lưu ý:** PhishMe (hiện là Cofense) là một giải pháp thương mại cung cấp các chương trình đào tạo và mô phỏng tấn công phishing cho người dùng cuối.

**PhishMe's** training programs aim to teach employees how to recognize and report phishing attempts, as well as how to protect their personal and professional accounts from these types of attacks.

The company's training programs can be customized to fit the needs of different organizations and can be delivered through a variety of mediums, including online courses, in-person training, and simulations.
**Lưu ý:** Việc đào tạo người dùng cuối (end-user training) là một biện pháp phòng vệ quan trọng của Blue Team để giảm rủi ro tấn công thông qua yếu tố con người.

Request a demo from [tại đây](https://go.cofense.com/live-demo/).

**Useful links:**

[Blog Cofense](https://cofense.com/blog/)

[Trung tâm Kiến thức Cofense](https://cofense.com/knowledge-center-hub/)

![image](https://user-images.githubusercontent.com/100603074/210669120-1b29007a-f7f6-40f6-922b-9b5b251f6447.png)

*Image used from https://cofense.com/product-services/phishme/*

**Giao tiếp và Cộng tác**
====================

Công cụ để phối hợp và giao tiếp với các thành viên trong nhóm trong suốt sự cố, bao gồm chat, email và phần mềm quản lý dự án.

### [🔙](#tool-list)[**Twitter**](https://twitter.com/)

**Twitter** is a great platform for sharing information about cyber security.
**Lưu ý:** Twitter là một nguồn thông tin mở (OSINT) rất phong phú và cập nhật về các mối đe dọa bảo mật, IoC mới, phân tích malware và các TTP mới nổi.

It's a platform that is widely used by security professionals, researchers, and experts, giving you access to an endless amount of new information.

Some great accounts to follow:

- [@vxunderground](https://twitter.com/vxunderground)
- [@Alh4zr3d](https://twitter.com/Alh4zr3d)
- [@3xp0rtblog](https://twitter.com/3xp0rtblog)
- [@C5pider](https://twitter.com/C5pider)
- [@_JohnHammond](https://twitter.com/_JohnHammond)
- [@mrd0x](https://twitter.com/mrd0x)
- [@TheHackersNews](https://twitter.com/TheHackersNews)
- [@pancak3lullz](https://twitter.com/pancak3lullz)
- [@GossiTheDog](https://twitter.com/GossiTheDog)
- [@briankrebs](https://twitter.com/briankrebs)
- [@SwiftOnSecurity](https://twitter.com/SwiftOnSecurity)
- [@schneierblog](https://twitter.com/schneierblog)
- [@mikko](https://twitter.com/mikko)
- [@campuscodi](https://twitter.com/campuscodi)
**Lưu ý:** Danh sách các tài khoản Twitter có ảnh hưởng hoặc chia sẻ nhiều nội dung liên quan đến an ninh mạng, rất đáng để Blue Team theo dõi để cập nhật tin tức và kỹ thuật mới.

### [🔙](#tool-list)[**Facebook ThreatExchange**](https://developers.facebook.com/docs/threat-exchange/getting-started)

**Facebook ThreatExchange** is a platform for security professionals to share and analyze information about cyber threats.
**Lưu ý:** Đây là một nền tảng chia sẻ IoC riêng tư (dành cho các thành viên đã được phê duyệt), cho phép các tổ chức chia sẻ các chỉ báo về mối đe dọa mà họ phát hiện với các thành viên khác để nâng cao nhận thức chung và khả năng phòng thủ của cộng đồng.

It was designed to help organizations better defend against threats by allowing them to share threat intelligence with each other in a private and secure way.

It is intended to be used by "**blue teams**", who are responsible for the security of an organization and work to prevent, detect, and respond to cyber threats.
**Lưu ý:** Là một kênh để Blue Team nhập IoC phát hiện trong quá trình điều tra và nhận IoC từ các tổ chức khác, hỗ trợ các hoạt động threat hunting và cập nhật biện pháp phòng thủ.

**Usage:**

To request access to **ThreatExchange**, you have to submit an application via [https://developers.facebook.com/products/threat-exchange/](https://developers.facebook.com/products/threat-exchange/).
**Lưu ý:** Cần đăng ký và được Facebook phê duyệt để tham gia nền tảng.

**Useful links:**

[Chào mừng đến với ThreatExchange!](https://developers.facebook.com/docs/threat-exchange/getting-started)

[Tổng quan giao diện ThreatExchange](https://developers.facebook.com/docs/threat-exchange/ui)

[Tham khảo API ThreatExchange](https://developers.facebook.com/docs/threat-exchange/reference/apis)

[GitHub - ThreatExchange](https://github.com/facebook/ThreatExchange/tree/main/python-threatexchange)
**Lưu ý:** ThreatExchange cung cấp API để tự động hóa việc nhập/xuất/tìm kiếm IoC, cho phép tích hợp với các công cụ hoặc platform TI nội bộ của tổ chức.
