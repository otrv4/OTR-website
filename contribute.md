---
layout: page
title: Contribute
tags: menu
permalink: /contribute/
---

<div class="container">
  <div class="about-text">
    <div class="flex-container">
      <div class="contact-item">
        <br><br>
        <a href="#contribute"><p>How to contribute</p></a>
      </div>
      <div class="contact-item">
        <br><br>
        <a href="#contact-points"><p>More contact points</p></a>
      </div>
      <div class="contact-item">
        <br><br>
        <a href="#sponsorship"><p>Sponsorship</p></a>
      </div>
      <div class="contact-item">
        <br><br>
        <a href="#jabber-service"><p>Jabber service</p></a>
      </div>
    </div>

  <div class="contribute">
    <a id="contribute"><h1><b>How to contribute</b></h1></a>
		<br>
		<p>This section should guide you through the initial steps of contributing to OTR. Thank you! Welcome, we're delighted to see you! :)</p>
		<p>If you have any questions, comments, doubts or concerns, please, feel free to reach us at the <a href="http://webchat.oftc.net/?randomnick=1&channels=otr&uio=d4" target="_blank" title="OTR IRC channel">#otr channel</a> on the OFTC IRC network. We also have an <a href="https://join.slack.com/t/otr-5b86249/shared_invite/zt-fpobxfsj-WA6StarxtcR1dIjWEaREgA" target="_blank" title="OTR slack channel">slack channel</a> for more contact. You can also contact us through our mailing list.</p>
		<p>For requests, suggestions and bug reports, please open an issue on our Gitlab, on the appropriate repository. If you want to fix a bug or suggest something, ask for mentoring to Sofía Celi at sofia@otr.im</p>
		<p><strong>A few things anyone can do</strong></p>
		<ul>
		  <li>Spread the word around OTR and its new version. Tell your friends!</li>
      <li>We always look for examples of how OTR is used or how or how can it be used. If you know, let us know!</li>
		</ul>
  </div>
  <br>

  <hr>
  <div class="contribute">
    <a id="contact-points"><h1><b>More contact points</b></h1></a>
		<br>
		<p>Our contact points are listed on the lovely footer; but we have more:</p>
		<ul>
		  <li><a href="https://lists.cypherpunks.ca/mailman/listinfo/otr-users" target="_blank" title="OTR User mailing list">User mailing list</a>: OTR has numerous users from all kinds of backgrounds, next to it being used by several hundred-thousands throughout the the world. Signup to the user mailinglist to help us improve its usability!</li>
                  <li><a href="https://lists.cypherpunks.ca/mailman/listinfo/otr-announce" target="_blank" title="OTR Announce mailing list">Announce mailinglist</a>: If you're interested in being notified when new releases are put out or want to follow the latest news. Please subscribe to the otr-announce mailinglist! </li>
		</ul>
  </div>
  <br>
  <hr>
  <div class="contribute">
    <a id="sponsorship"><h1><b>Sponsorship</b></h1></a>
    <br>
    <p>OTR (in its version 4) is sponsored by the <a href="https://nlnet.nl/" target="_blank" title="NLNet Foundation Website">NLNet Foundation</a>. Funding was provided through the <a href="https://www.ngi.eu/ngi-projects/ngi-zero/" target="_blank" title="NGIO Privacy Enhancing Technologies Fund Website">NGI0 Privacy Enhancing Technologies Fund</a>, a fund established by NLnet with financial support from the European Commission’s Next Generation Internet program, under the aegis of DG Communications Networks, Content and Technology under grant agreement #825310.</p>
  </div>

  <hr>
  <div class="contribute">
    <a id="jabber-service"><h1><b>Our own jabber service</b></h1></a>
    <h5>OTR.im chat</h5>
    <br>
    <p>OTR.im offers a free and secure Jabber service that anyone can use by registering an account through your favorite chat client.</p>
    <p>➛ jabber.otr.im</p>
    <p>It is also possible to connect to it through our Tor hidden service:</p>
    <p>➛ 5rgdtlawqkcplz75.onion</p>
    <p>In order to configure a Jabber client, you need this information:</p>
    <p><code>
       <p>Protocol: jabber or xmpp </p>
       <p>Account: username@jabber.otr.im </p>
    </code></p>
    <p>Our Jabber server requires a secure SSL/TLS connection. We use Let's Encrypt since March 22nd, 2016 thus you should expect a valid signed certificate for jabber.otr.im.</p>
    <p>Finally, this server has a special quirk. It forces communication to be OTR encrypted, thus cleartext messages between clients is impossible. With the help of Riseup, we have developed a prosody plugin to achieve mandatory OTR communication.</p>
    <h2>Data Retention</h2>
    <p>What data does OTR.im can see and can not see with this Jabber server:</p>
    <p>First of all, this server is setup with full disk encryption (FDE) so all that we store is only on an encrypted disk. We use a LUKS device for this. Secondly, logging is completely disabled on the Jabber server, even error logs.</p>
    <p>In case of a seizure, if the server is powered off, the FDE will protect all data. If the server is kept online, see the 'What we can see?' section below.</p>
    <h2>What we CAN see?</h2>
    <ul>
      <li>Your username and SHA1 hash of the password are stored on the server.</li>
      <li>vCard if you supply one.</li>
      <li>Your IP address. To avoid this, use our Tor hidden service.</li>
      <li>Offline messages. Any messages you send to an offline contact will be stored encrypted on the server until the contact shows up:</li>
      <ul>
        <li>Encrypted content with OTR.</li>
        <li>Destination contact address.</li>
        <li>Timestamp of the messages sent.</li>
      </ul>
      <li>Your roster. For each contact, we see:</li>
      <ul>
        <li>Jabber address (for example: keith@jabber.boozallen.com)</li>
        <li>Name of the contact (if set)</li>
        <li>Group it belongs to (if any)</li>
      </ul>
    </ul>
    <br>

    <h2>What we DO NOT see?</h2>
    <ul>
      <li>The Message content. Mandatory OTR makes it that we can't read content of your messages.</li>
      <li>No logs, except for what our prosody server usually tell us.</li>
      <li>We don't keep any timing metadata such as when you connect or disconnect.</li>
    </ul>
  </div>
</div>
