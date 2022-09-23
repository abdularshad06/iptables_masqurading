# iptables_masqurading



# iptables -A FORWARD -i br0 -o em2 -j ACCEPT
# iptables -A FORWARD -i em2 -o br0 -m state --state ESTABLISHED,RELATED -j ACCEPT
# iptables -t nat -A POSTROUTING -o em2 -j MASQUERADE
