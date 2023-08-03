<p align="center">
  <a href="#build-framework">
   <img src="https://raw.githubusercontent.com/armbian/build/master/.github/armbian-logo.png" alt="Armbian logo" width="144">
  </a><br>
  <strong>Armbian OS</strong><br>
<br>
<a href=https://github.com/armbian/os/actions/workflows/complete-artifact-matrix-all.yml><img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/armbian/os/complete-artifact-matrix-all.yml?logo=githubactions&label=Artifacts%20make&style=for-the-badge&branch=main"></a>
<a href=https://github.com/armbian/os/actions/workflows/repository-update.yml><img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/armbian/os/repository-update.yml?logo=githubactions&label=Repository%20update&style=for-the-badge&branch=main"></a>
<a href=https://github.com/armbian/os#latest-smoke-tests-results><img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/armbian/os/smoke-tests.yml?logo=githubactions&label=Smoke%20tests&style=for-the-badge&branch=main"></a>
</p>


# What does this project do?

- Keeps build framework [packages artifacts](https://github.com/orgs/armbian/packages) cache up to date
- Keeps stable [apt.armbian.com](https://apt.armbian.com) and nightly [beta.armbian.com](https://beta.armbian.com) packages repository up to date
- Builds [nightly](https://github.com/armbian/os/releases) and [stable images](https://www.armbian.com/download/) and uploads them to Armbian CDN
- Keep synchronizing the selection of [3rd party](external) applications with Armbian repositories
- Tests install of all packages added onto stable and testing Debian and Ubuntu releases

# When is this happening?

- Artifacts cache is updated every eight hours, starting at 0:00 AM UTC
- Repository update is updated once per day, at 3:00 AM UTC
- Smoke tests is executed after **repository update** is finished.
- Nightly images are build once per day, at 5:00 AM UTC
- Manually, when Armbian [release manager](https://github.com/orgs/armbian/teams/release-manager) executes a build action

# Latest smoke tests results:

- installs kernels, dtb and headers that are defined and supported by the board
- runs network and computing performance tests (7z benchmark)
- store armbianmonitor logs

<!--START_SECTION:data-section-->
<table width="100%"><tr><td align="left"><a href="https://paste.armbian.com/wisodahopu">Tinker Board</a></td><td align="left">2023-08-03 18:21:14</td><td align=left>current</td><td align=right>2022.04</td><td align=right>6.1.42-rockchip</td><td align=right>89</td><td align=right>5034</td></tr><tr><td align="left"><a href="https://paste.armbian.com/fihefigilo">Tinker Board</a></td><td align="left">2023-08-03 18:25:22</td><td align=left>edge</td><td align=right>2022.04</td><td align=right>6.4.7-rockchip</td><td align=right>90</td><td align=right>4854</td></tr><tr><td align="left"><a href="https://paste.armbian.com/qevewakica">Espressobin</a></td><td align="left">2023-08-03 18:22:27</td><td align=left>current</td><td align=right></td><td align=right>5.15.123-mvebu64</td><td align=right>880</td><td align=right>1127</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Espressobin</a></td><td align="left">2023-08-03 18:31:34</td><td align=left>edge</td><td align=right></td><td align=right>6.1.42-mvebu64</td><td align=right>880</td><td align=right>1112</td></tr><tr><td align="left"><a href="https://paste.armbian.com/coxukevinu">Pine H64</a></td><td align="left">2023-08-03 18:16:41</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi64</td><td align=right>842</td><td align=right>3712</td></tr><tr><td align="left"><a href="https://paste.armbian.com/tafigowava">Pine H64</a></td><td align="left">2023-08-03 18:21:21</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi64</td><td align=right>868</td><td align=right>3653</td></tr><tr><td align="left"><a href="https://paste.armbian.com/useqonurez">Pine H64</a></td><td align="left">2023-08-03 18:25:57</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi64</td><td align=right>870</td><td align=right>3662</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">UEFI x86</a></td><td align="left">2023-08-03 18:26:29</td><td align=left>legacy</td><td align=right></td><td align=right>5.15.123-x86</td><td align=right>831</td><td align=right>4600</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">UEFI x86</a></td><td align="left">2023-08-03 18:31:22</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-x86</td><td align=right>770</td><td align=right>4612</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">UEFI x86</a></td><td align="left">2023-08-03 18:36:52</td><td align=left>edge</td><td align=right></td><td align=right>6.4.7-x86</td><td align=right>824</td><td align=right>4719</td></tr><tr><td align="left"><a href="https://paste.armbian.com/opevewulim">Banana Pi M5</a></td><td align="left">2023-08-03 18:16:27</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-meson64</td><td align=right>718</td><td align=right>5520</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ogufoxiyil">Banana Pi M5</a></td><td align="left">2023-08-03 18:21:22</td><td align=left>edge</td><td align=right></td><td align=right>6.4.7-meson64</td><td align=right>870</td><td align=right>5505</td></tr><tr><td align="left"><a href="https://paste.armbian.com/yipumexuyu">Odroid C2</a></td><td align="left">2023-08-03 18:15:08</td><td align=left>current</td><td align=right>2022.01</td><td align=right>6.1.42-meson64</td><td align=right>880</td><td align=right>3890</td></tr><tr><td align="left"><a href="https://paste.armbian.com/imujunozuk">Odroid C2</a></td><td align="left">2023-08-03 18:19:55</td><td align=left>edge</td><td align=right>2022.01</td><td align=right>6.4.7-meson64</td><td align=right>850</td><td align=right>3899</td></tr><tr><td align="left"><a href="https://paste.armbian.com/uyubukuyen">Orange Pi 4 LTS</a></td><td align="left">2023-08-03 18:14:26</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-rockchip64</td><td align=right>950</td><td align=right>5329</td></tr><tr><td align="left"><a href="https://paste.armbian.com/paqoriwuqa">Orange Pi 4 LTS</a></td><td align="left">2023-08-03 18:19:36</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-rockchip64</td><td align=right>960</td><td align=right>3807</td></tr><tr><td align="left"><a href="https://paste.armbian.com/miluyifopo">NanoPi R6S</a></td><td align="left">2023-08-03 18:13:38</td><td align=left>legacy</td><td align=right>2017.09</td><td align=right>5.10.160-rk35xx</td><td align=right>2241</td><td align=right>15801</td></tr><tr><td align="left"><a href="https://paste.armbian.com/fubonimoda">Cubieboard 1</a></td><td align="left">2023-08-03 18:26:39</td><td align=left>legacy</td><td align=right>2022.07</td><td align=right>5.15.123-sunxi</td><td align=right>78</td><td align=right>579</td></tr><tr><td align="left"><a href="https://paste.armbian.com/apatoperud">Cubieboard 1</a></td><td align="left">2023-08-03 18:36:53</td><td align=left>current</td><td align=right>2022.07</td><td align=right>6.1.42-sunxi</td><td align=right>77</td><td align=right>560</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Cubieboard 1</a></td><td align="left">2023-08-03 18:47:57</td><td align=left>edge</td><td align=right>2022.07</td><td align=right>6.4.7-sunxi</td><td align=right>75</td><td align=right>558</td></tr><tr><td align="left"><a href="https://paste.armbian.com/inayiyomiv">Orange Pi 3 LTS</a></td><td align="left">2023-08-03 18:14:20</td><td align=left>current</td><td align=right>2022.07</td><td align=right>6.1.42-sunxi64</td><td align=right>866</td><td align=right>3934</td></tr><tr><td align="left"><a href="https://paste.armbian.com/futimegoko">Orange Pi 3 LTS</a></td><td align="left">2023-08-03 18:18:35</td><td align=left>edge</td><td align=right>2022.07</td><td align=right>6.4.7-sunxi64</td><td align=right>870</td><td align=right>3895</td></tr><tr><td align="left"><a href="https://paste.armbian.com/umuwetaqas">Odroid C4</a></td><td align="left">2023-08-03 18:16:07</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-meson64</td><td align=right>780</td><td align=right>5639</td></tr><tr><td align="left"><a href="https://paste.armbian.com/atidedusuk">Odroid C4</a></td><td align="left">2023-08-03 18:22:11</td><td align=left>edge</td><td align=right></td><td align=right>6.4.7-meson64</td><td align=right>808</td><td align=right>5627</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Rockpi 4B</a></td><td align="left">2023-08-03 18:14:39</td><td align=left>legacy</td><td align=right>2022.07</td><td align=right>4.4.213-rockchip64</td><td align=right>833</td><td align=right>6036</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Rockpi 4B</a></td><td align="left">2023-08-03 18:19:07</td><td align=left>current</td><td align=right>2022.07</td><td align=right>6.1.42-rockchip64</td><td align=right>930</td><td align=right>6268</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Rockpi 4B</a></td><td align="left">2023-08-03 18:23:53</td><td align=left>edge</td><td align=right>2022.07</td><td align=right>6.3.13-rockchip64</td><td align=right>960</td><td align=right>6288</td></tr><tr><td align="left"><a href="https://paste.armbian.com/uwonayoxap">NanoPi M4</a></td><td align="left">2023-08-03 18:14:36</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-rockchip64</td><td align=right>880</td><td align=right>6729</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ifiyobuqik">NanoPi M4</a></td><td align="left">2023-08-03 18:18:55</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-rockchip64</td><td align=right>880</td><td align=right>6639</td></tr><tr><td align="left"><a href="https://paste.armbian.com/apeserosot">Le potato</a></td><td align="left">2023-08-03 18:16:31</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-meson64</td><td align=right>90</td><td align=right>3804</td></tr><tr><td align="left"><a href="https://paste.armbian.com/vamicurote">Le potato</a></td><td align="left">2023-08-03 18:22:41</td><td align=left>edge</td><td align=right></td><td align=right>6.4.7-meson64</td><td align=right>91</td><td align=right>3805</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Raspberry Pi 4</a></td><td align="left">2023-08-03 18:23:49</td><td align=left>legacy</td><td align=right></td><td align=right>6.3.13-bcm2711</td><td align=right>90</td><td align=right>1788</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Raspberry Pi 4</a></td><td align="left">2023-08-03 18:30:52</td><td align=left>current</td><td align=right></td><td align=right>6.3.13-bcm2711</td><td align=right>91</td><td align=right>1795</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Raspberry Pi 4</a></td><td align="left">2023-08-03 18:38:02</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-bcm2711</td><td align=right>90</td><td align=right>1728</td></tr><tr><td align="left"><a href="https://paste.armbian.com/axepixomox">Orange Pi R1</a></td><td align="left">2023-08-03 18:15:05</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi</td><td align=right>90</td><td align=right>2806</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ekucebuyow">Orange Pi R1</a></td><td align="left">2023-08-03 18:19:06</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>90</td><td align=right>2438</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Banana Pi Pro</a></td><td align="left">2023-08-03 18:23:55</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi</td><td align=right>533</td><td align=right>1038</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Banana Pi Pro</a></td><td align="left">2023-08-03 18:32:14</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi</td><td align=right>424</td><td align=right>1020</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Banana Pi Pro</a></td><td align="left">2023-08-03 18:41:07</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>361</td><td align=right>1014</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ecehelojec">ZeroPi</a></td><td align="left">2023-08-03 18:26:00</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi</td><td align=right>652</td><td align=right>2548</td></tr><tr><td align="left"><a href="https://paste.armbian.com/cizovapeye">ZeroPi</a></td><td align="left">2023-08-03 18:31:23</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>552</td><td align=right>2537</td></tr><tr><td align="left"><a href="https://paste.armbian.com/uruwuleqoy">Cubietruck</a></td><td align="left">2023-08-03 18:25:10</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi</td><td align=right>597</td><td align=right>1028</td></tr><tr><td align="left"><a href="https://paste.armbian.com/orugozemeh">Cubietruck</a></td><td align="left">2023-08-03 18:34:04</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi</td><td align=right>717</td><td align=right>1015</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ezosuviwis">Cubietruck</a></td><td align="left">2023-08-03 18:43:15</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>584</td><td align=right>1012</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ukopazilur">NanoPi R4S</a></td><td align="left">2023-08-03 18:14:44</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-rockchip64</td><td align=right>880</td><td align=right>6462</td></tr><tr><td align="left"><a href="https://paste.armbian.com/hutesozobu">NanoPi R4S</a></td><td align="left">2023-08-03 18:19:21</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-rockchip64</td><td align=right>800</td><td align=right>6475</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ifigegijil">Odroid N2</a></td><td align="left">2023-08-03 18:13:00</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-meson64</td><td align=right>870</td><td align=right>8932</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ovipomuvac">Odroid N2</a></td><td align="left">2023-08-03 18:16:10</td><td align=left>edge</td><td align=right></td><td align=right>6.4.7-meson64</td><td align=right>900</td><td align=right>8933</td></tr><tr><td align="left"><a href="https://paste.armbian.com/aqebirikix">Clearfog Pro</a></td><td align="left">2023-08-03 18:14:13</td><td align=left>current</td><td align=right>2018.01</td><td align=right>6.1.42-mvebu</td><td align=right>820</td><td align=right>2229</td></tr><tr><td align="left"><a href="https://paste.armbian.com/">Clearfog Pro</a></td><td align="left">2023-08-03 18:18:12</td><td align=left>edge</td><td align=right>2018.01</td><td align=right>6.2.16-mvebu</td><td align=right>830</td><td align=right>2235</td></tr><tr><td align="left"><a href="https://paste.armbian.com/cohicuhesi">NanoPi Neo 3</a></td><td align="left">2023-08-03 18:17:24</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-rockchip64</td><td align=right>872</td><td align=right>2335</td></tr><tr><td align="left"><a href="https://paste.armbian.com/egexuwadop">NanoPi Neo 3</a></td><td align="left">2023-08-03 18:24:58</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-rockchip64</td><td align=right>900</td><td align=right>1904</td></tr><tr><td align="left"><a href="https://paste.armbian.com/gadafetuco">ODROID M1</a></td><td align="left">2023-08-03 18:14:47</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-rk3568-odroid</td><td align=right>950</td><td align=right>5338</td></tr><tr><td align="left"><a href="https://paste.armbian.com/xivosubize">Orange Pi Zero</a></td><td align="left">2023-08-03 18:18:55</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi</td><td align=right>90</td><td align=right>2344</td></tr><tr><td align="left"><a href="https://paste.armbian.com/akaxaciwit">Orange Pi Zero</a></td><td align="left">2023-08-03 18:23:29</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi</td><td align=right>91</td><td align=right>2581</td></tr><tr><td align="left"><a href="https://paste.armbian.com/kupajovume">Orange Pi Zero</a></td><td align="left">2023-08-03 18:28:19</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>90</td><td align=right>2296</td></tr><tr><td align="left"><a href="https://paste.armbian.com/winigerimo">Orange Pi Zero Plus</a></td><td align="left">2023-08-03 18:18:24</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi64</td><td align=right>816</td><td align=right>2538</td></tr><tr><td align="left"><a href="https://paste.armbian.com/muxevosira">Orange Pi Zero Plus</a></td><td align="left">2023-08-03 18:23:38</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi64</td><td align=right>810</td><td align=right>2519</td></tr><tr><td align="left"><a href="https://paste.armbian.com/qusejalefu">Orange Pi Zero Plus</a></td><td align="left">2023-08-03 18:28:45</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi64</td><td align=right>840</td><td align=right>2517</td></tr><tr><td align="left"><a href="https://paste.armbian.com/govoqoriqu">Tinker Board 2</a></td><td align="left">2023-08-03 18:23:25</td><td align=left>current</td><td align=right>2021.07</td><td align=right>6.1.42-rockchip64</td><td align=right>889</td><td align=right>6824</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ofunohukam">Tinker Board 2</a></td><td align="left">2023-08-03 18:27:41</td><td align=left>edge</td><td align=right>2021.07</td><td align=right>6.3.13-rockchip64</td><td align=right>805</td><td align=right>6720</td></tr><tr><td align="left"><a href="https://paste.armbian.com/yadigozoko">A64 OLinuXino</a></td><td align="left">2023-08-03 18:28:41</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi64</td><td align=right>709</td><td align=right>2526</td></tr><tr><td align="left"><a href="https://paste.armbian.com/oxadadumok">A64 OLinuXino</a></td><td align="left">2023-08-03 18:37:15</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi64</td><td align=right>633</td><td align=right>2787</td></tr><tr><td align="left"><a href="https://paste.armbian.com/qagonujeze">A64 OLinuXino</a></td><td align="left">2023-08-03 18:46:35</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi64</td><td align=right>709</td><td align=right>2795</td></tr><tr><td align="left"><a href="https://paste.armbian.com/afovinocoy">Khadas VIM2</a></td><td align="left">2023-08-03 18:15:51</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-meson64</td><td align=right>960</td><td align=right>6260</td></tr><tr><td align="left"><a href="https://paste.armbian.com/ezozurufas">Khadas VIM2</a></td><td align="left">2023-08-03 18:21:26</td><td align=left>edge</td><td align=right></td><td align=right>6.4.7-meson64</td><td align=right>880</td><td align=right>6221</td></tr><tr><td align="left"><a href="https://paste.armbian.com/awoxiyezah">Orange Pi R1 Plus LTS</a></td><td align="left">2023-08-03 18:17:45</td><td align=left>current</td><td align=right></td><td align=right>6.1.42-rockchip64</td><td align=right>431</td><td align=right>1931</td></tr><tr><td align="left"><a href="https://paste.armbian.com/uzigalagac">Orange Pi R1 Plus LTS</a></td><td align="left">2023-08-03 18:25:20</td><td align=left>edge</td><td align=right></td><td align=right>6.3.13-rockchip64</td><td align=right>700</td><td align=right>1938</td></tr><tr><td align="left"><a href="https://paste.armbian.com/gulisijabo">Orange Pi Zero Plus 2</a></td><td align="left">2023-08-03 18:20:56</td><td align=left>legacy</td><td align=right>2023.07</td><td align=right>5.15.123-sunxi</td><td align=right>39</td><td align=right>2439</td></tr><tr><td align="left"><a href="https://paste.armbian.com/vadiguhoso">Orange Pi Zero Plus 2</a></td><td align="left">2023-08-03 18:26:34</td><td align=left>current</td><td align=right>2023.07</td><td align=right>6.1.42-sunxi</td><td align=right>37</td><td align=right>2687</td></tr><tr><td align="left"><a href="https://paste.armbian.com/coyugivegi">Orange Pi Zero Plus 2</a></td><td align="left">2023-08-03 18:33:14</td><td align=left>edge</td><td align=right>2023.07</td><td align=right>6.4.7-sunxi</td><td align=right>40</td><td align=right>2408</td></tr></table>
<!--END_SECTION:data-section-->

## Would you like to join spare hardware to this automated testings?

All you need to do is:

- deploy any latest Armbian image to hardware
- provide IP address
- [contact us](https://www.armbian.com/contact/)

Device has to be always on and easily accesible for you to re-image in case of failed upgrade.

## Development

- [Pull request](https://github.com/armbian/build/pulls)
- [Weekly developers meetings](https://forum.armbian.com/events/)
- [Forums for developers](https://forum.armbian.com/forum/4-advanced-users-development/)

## OS download

- [Download](https://www.armbian.com/download/)

## Support

- [Using Armbian](https://forum.armbian.com/forum/23-using-armbian/)

## Contact

- [Forums](https://forum.armbian.com) for Participate in Armbian
- IRC: `#armbian` on Libera.chat
- Discord: [https://discord.gg/armbian](https://discord.gg/armbian)
- Follow [@armbian](https://twitter.com/armbian) on Twitter, [Fosstodon](https://fosstodon.org/@armbian) or [LinkedIn](https://www.linkedin.com/company/armbian).
- Bugs: [issues](https://github.com/armbian/build/issues) / [JIRA](https://armbian.atlassian.net/jira/dashboards/10000)
- Office hours: [Wednesday, 12 midday, 18 afternoon, CET](https://calendly.com/armbian/office-hours)

## License

This software is published under the GPL-2.0 License license.
