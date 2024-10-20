# DHCP

DORA-Prozess im Detail

    Discover: Der DHCP-Client sendet ein Broadcast-Paket an alle verfügbaren DHCP-Ports bzw. Server. Dies geschieht mit einer Anforderung zur IP-Adressvergabe.

    Offer: Einer oder mehrere Server antworten mit einem Angebot. Dieses enthält eine freie IP-Adresse und andere Konfigurationsparameter.

    Request: Der Client wählt das beste Angebot aus. Er sendet eine Anforderungsnachricht an den jeweiligen Port für DHCP.

    Acknowledge: Der ausgewählte DHCP-Server bestätigt die Zuweisung. Der Client speichert die erhaltenen Konfigurationsdaten lokal.

# ASN Numbering

Within the data center each BGP router is identified by a private autonomous system number (ASN). This ASN is used for internal communication. The default is to have 2-byte ASN. To avoid having to find workarounds in case the ASN address space is exhausted, a 4-byte ASN that supports up to 95 million ASNs (4200000000–4294967294) is used from the beginning.

ASN numbering in a CLOS topology should follow a model to avoid routing problems (path hunting) due to it's redundant nature. Within a CLOS topology the following ASN numbering model is suggested to solve path hunting problems:

1.  Leaves have unique ASN
2.  Spines share an ASN
3.  Exit switches share an ASN
