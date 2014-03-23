AUTOMAKE_OPTIONS = subdir-objects
AM_CFLAGS = -DNDEBUG=1 -std=gnu99 -Wno-unused-value -Wno-parentheses
AM_CFLAGS += -I"lwip/src/include/ipv4" -I"lwip/src/include/ipv6" -I"lwip/src/include" -I"lwip/custom"
AM_CFLAGS += -DBADVPN_BREACTOR_BADVPN -DBADVPN_FREEBSD -DBADVPN_THREADWORK_USE_PTHREAD -DBADVPN_THREAD_SAFE=1 -DBADVPN_USE_KEVENT -DBADVPN_USE_SYSLOG -DBADVPN_LITTLE_ENDIAN -DBADVPN_SOCKS_UDP_RELAY -DBADVPN_LIBTSOCKS -DTARGET_LIBTSOCKS

noinst_LTLIBRARIES = libtsocks.la
libtsocks_la_LDFLAGS = -static
libtsocks_la_SOURCES = tun2socks/tun2socks.c \
	base/BLog_syslog.c \
	system/BReactor_badvpn.c \
	system/BSignal.c \
	system/BConnection_unix.c \
	system/BTime.c \
	system/BUnixSignal.c \
	system/BNetwork.c \
	system/BDatagram_unix.c \
	flow/StreamRecvInterface.c \
	flow/PacketRecvInterface.c \
	flow/PacketPassInterface.c \
	flow/StreamPassInterface.c \
	flow/SinglePacketBuffer.c \
	flow/BufferWriter.c \
	flow/PacketBuffer.c \
	flow/PacketStreamSender.c \
	flow/PacketPassConnector.c \
	flow/PacketProtoFlow.c \
	flow/PacketPassFairQueue.c \
	flow/PacketProtoEncoder.c \
	flow/PacketProtoDecoder.c \
	socksclient/BSocksClient.c \
	tuntap/BTap.c \
	lwip/src/core/timers.c \
	lwip/src/core/udp.c \
	lwip/src/core/memp.c \
	lwip/src/core/init.c \
	lwip/src/core/pbuf.c \
	lwip/src/core/tcp.c \
	lwip/src/core/tcp_out.c \
	lwip/src/core/netif.c \
	lwip/src/core/def.c \
	lwip/src/core/mem.c \
	lwip/src/core/tcp_in.c \
	lwip/src/core/stats.c \
	lwip/src/core/inet_chksum.c \
	lwip/src/core/ipv4/icmp.c \
	lwip/src/core/ipv4/ip4.c \
	lwip/src/core/ipv4/ip4_addr.c \
	lwip/src/core/ipv4/ip_frag.c \
	lwip/src/core/ipv6/ip6.c \
	lwip/src/core/ipv6/nd6.c \
	lwip/src/core/ipv6/icmp6.c \
	lwip/src/core/ipv6/ip6_addr.c \
	lwip/src/core/ipv6/ip6_frag.c \
	lwip/custom/sys.c \
	base/DebugObject.c \
	base/BLog.c \
	base/BPending.c \
	flowextra/PacketPassInactivityMonitor.c \
	tun2socks/SocksUdpGwClient.c \
	udpgw_client/UdpGwClient.c
