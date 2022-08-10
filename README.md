# RDPWrap-Win10last--win11

; RDP Wrapper Library configuration
; Do not modify without special knowledge
; Edited by sebaxakerhtc

[Main]
Updated=2022-08-04
LogFile=\rdpwrap.txt
SLPolicyHookNT60=1
SLPolicyHookNT61=1

[SLPolicy]
TerminalServices-RemoteConnectionManager-AllowRemoteConnections=1
TerminalServices-RemoteConnectionManager-AllowMultipleSessions=1
TerminalServices-RemoteConnectionManager-AllowAppServerMode=1
TerminalServices-RemoteConnectionManager-AllowMultimon=1
TerminalServices-RemoteConnectionManager-MaxUserSessions=0
TerminalServices-RemoteConnectionManager-ce0ad219-4670-4988-98fb-89b14c2f072b-MaxSessions=0
TerminalServices-RemoteConnectionManager-45344fe7-00e6-4ac6-9f01-d01fd4ffadfb-MaxSessions=2
TerminalServices-RDP-7-Advanced-Compression-Allowed=1
TerminalServices-RemoteConnectionManager-45344fe7-00e6-4ac6-9f01-d01fd4ffadfb-LocalOnly=0
TerminalServices-RemoteConnectionManager-8dc86f1d-9969-4379-91c1-06fe1dc60575-MaxSessions=1000
TerminalServices-DeviceRedirection-Licenses-TSEasyPrintAllowed=1
TerminalServices-DeviceRedirection-Licenses-PnpRedirectionAllowed=1
TerminalServices-DeviceRedirection-Licenses-TSMFPluginAllowed=1
TerminalServices-RemoteConnectionManager-UiEffects-DWMRemotingAllowed=1

[PatchCodes]
nop=90
Zero=00
jmpshort=EB
nopjmp=90E9
CDefPolicy_Query_edx_ecx=BA000100008991200300005E90
CDefPolicy_Query_eax_rcx_jmp=B80001000089813806000090EB
CDefPolicy_Query_eax_esi=B80001000089862003000090
CDefPolicy_Query_eax_rdi=B80001000089873806000090
CDefPolicy_Query_eax_ecx=B80001000089812003000090
CDefPolicy_Query_eax_ecx_jmp=B800010000898120030000EB0E
CDefPolicy_Query_eax_rcx=B80001000089813806000090
CDefPolicy_Query_edi_rcx=BF0001000089B938060000909090
; new patch by sebaxakerhtc
CDefPolicy_Query_eax_rdi_jmp=B800010000898738060000EB0D

[6.0.6000.16386]
SingleUserPatch.x86=1
SingleUserOffset.x86=160BF
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=65E3E
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=15CD8
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=5C88F
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.0.6001.18000]
SingleUserPatch.x86=1
SingleUserOffset.x86=185E4
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=70DBA
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=17FD8
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=65BD7
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.0.6002.18005]
SingleUserPatch.x86=1
SingleUserOffset.x86=17FA8
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=70FF6
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=179C0
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=65E83
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.0.6002.19214]
SingleUserPatch.x86=1
SingleUserOffset.x86=17FC4
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=712AA
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=179B8
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=65FF7
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.0.6001.22286]
SingleUserPatch.x86=1
SingleUserOffset.x86=185E4
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=70DDE
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=17FD8
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=65C01
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.0.6001.22323]
SingleUserPatch.x86=1
SingleUserOffset.x86=185E4
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=70DFA
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=17FD8
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=65C1D
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.0.6001.22357]
SingleUserPatch.x86=1
SingleUserOffset.x86=185E4
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=70DFA
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=17FD8
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=65C1D
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.0.6001.22801]
SingleUserPatch.x86=1
SingleUserOffset.x86=185F8
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=71ADA
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=18010
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=666AD
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.0.6002.22515]
SingleUserPatch.x86=1
SingleUserOffset.x86=17FA8
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=71AFA
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=179C0
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=6675D
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.0.6002.22641]
SingleUserPatch.x86=1
SingleUserOffset.x86=17FA8
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=71AFA
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=179C0
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=6675D
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.0.6002.22790]
SingleUserPatch.x86=1
SingleUserOffset.x86=17FA8
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=71B02
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=179C0
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=66765
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.0.6002.23521]
SingleUserPatch.x86=1
SingleUserOffset.x86=17FB4
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=71EAA
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=179CC
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=669CB
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.0.6003.20482]
SingleUserPatch.x86=1
SingleUserOffset.x86=17FC4
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=71F8A
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=179DC
DefPolicyCode.x86=CDefPolicy_Query_edx_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=66B65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx_jmp

[6.1.7600.16385]
SingleUserPatch.x86=1
SingleUserOffset.x86=19E25
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17D96
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=196F3
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17AD2
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7600.20621]
SingleUserPatch.x86=1
SingleUserOffset.x86=19E1D
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17DC2
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=196EB
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17ADE
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7600.20890]
SingleUserPatch.x86=1
SingleUserOffset.x86=19E2D
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17DF2
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=196FB
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17B0E
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7600.21316]
SingleUserPatch.x86=1
SingleUserOffset.x86=19E2D
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17E3E
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=196FB
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17B5E
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7600.21420]
SingleUserPatch.x86=1
SingleUserOffset.x86=19EF5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17D56
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19761
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17B3E
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.17514]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A49D
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=180E2
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19D53
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17D8A
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.18540]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A4E5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=18006
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19D9F
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17C82
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.18637]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A4DD
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=180FA
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19DBB
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17DC6
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.21650]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A49D
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=180BE
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19D53
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17D5A
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.21866]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A49D
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=180BE
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19D53
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17D5A
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.22104]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A49D
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=180C6
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19D53
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17D5E
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.22213]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A5AD
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17F26
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19DB1
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17D06
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.22435]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A5BD
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17F36
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19DB1
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17D16
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.22476]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A5CD
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17F56
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19DC1
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17D52
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.22750]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A655
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17E8E
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19E21
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17C92
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.22843]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A655
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17F96
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19E25
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17D6E
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.23403]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A65D
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17F62
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19E29
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17CE2
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.24234]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A675
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17F56
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19E41
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17D2E
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.24326]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A675
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17F1E
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19E41
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17CEE
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.24402]
SingleUserPatch.x86=1
SingleUserOffset.x86=1A675
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17F26
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=19E41
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17CFE
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.1.7601.25757]
SingleUserPatch.x64=1
SingleUserOffset.x64=17F86
; We'll use a method by Stas'M
; But for me it should be A97F86
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17D8A
; We'll use method by Stas'M
; But for me it should be A97D8A
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi

[6.2.8102.0]
SingleUserPatch.x86=1
SingleUserOffset.x86=F7E9
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=D840
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=E47C
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=D3E6
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi
SLPolicyInternal.x86=1
SLPolicyOffset.x86=1B909
SLPolicyFunc.x86=New_Win8SL
SLPolicyInternal.x64=1
SLPolicyOffset.x64=1A484
SLPolicyFunc.x64=New_Win8SL

[6.2.8250.0]
SingleUserPatch.x86=1
SingleUserOffset.x86=159C9
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=11E74
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=13520
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1187A
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi
SLPolicyInternal.x86=1
SLPolicyOffset.x86=1A0A9
SLPolicyFunc.x86=New_Win8SL_CP
SLPolicyInternal.x64=1
SLPolicyOffset.x64=18FAC
SLPolicyFunc.x64=New_Win8SL

[6.2.8400.0]
SingleUserPatch.x86=1
SingleUserOffset.x86=15482
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=20824
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=13E48
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1F102
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi
SLPolicyInternal.x86=1
SLPolicyOffset.x86=19629
SLPolicyFunc.x86=New_Win8SL
SLPolicyInternal.x64=1
SLPolicyOffset.x64=2492C
SLPolicyFunc.x64=New_Win8SL

[6.2.9200.16384]
SingleUserPatch.x86=1
SingleUserOffset.x86=15552
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=2BAA8
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=13F08
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=2A31A
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi
SLPolicyInternal.x86=1
SLPolicyOffset.x86=19559
SLPolicyFunc.x86=New_Win8SL
SLPolicyInternal.x64=1
SLPolicyOffset.x64=21FA8
SLPolicyFunc.x64=New_Win8SL

[6.2.9200.17048]
SingleUserPatch.x86=1
SingleUserOffset.x86=20592
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=20948
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=1F408
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1F206
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi
SLPolicyInternal.x86=1
SLPolicyOffset.x86=17059
SLPolicyFunc.x86=New_Win8SL
SLPolicyInternal.x64=1
SLPolicyOffset.x64=24570
SLPolicyFunc.x64=New_Win8SL

[6.2.9200.21166]
SingleUserPatch.x86=1
SingleUserOffset.x86=1557A
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=2BAF8
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=13F30
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=2A3B6
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi
SLPolicyInternal.x86=1
SLPolicyOffset.x86=19581
SLPolicyFunc.x86=New_Win8SL
SLPolicyInternal.x64=1
SLPolicyOffset.x64=21FD0
SLPolicyFunc.x64=New_Win8SL

[6.2.9200.22715]
; x86-Offsets are not safe (determined without symbols)
SingleUserPatch.x86=1
SingleUserOffset.x86=155B2
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=2BAE4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=13F68
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
DefPolicyPatch.x64=1
DefPolicyOffset.x64=2A396
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi
SLPolicyInternal.x86=1
SLPolicyOffset.x86=195B9
SLPolicyFunc.x86=New_Win8SL
SLPolicyInternal.x64=1
SLPolicyOffset.x64=21F90
SLPolicyFunc.x64=New_Win8SL

[6.2.9200.22977]
; no x64-version
SingleUserPatch.x86=1
SingleUserOffset.x86=155B2
SingleUserCode.x86=nop
DefPolicyPatch.x86=1
DefPolicyOffset.x86=13F68
DefPolicyCode.x86=CDefPolicy_Query_eax_esi
SLPolicyInternal.x86=1
SLPolicyOffset.x86=195B9
SLPolicyFunc.x86=New_Win8SL

[6.2.9200.23509]
; new patch apply
SingleUserPatch.x64=1
SingleUserOffset.x64=8E110
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=7B292
DefPolicyCode.x64=CDefPolicy_Query_eax_rdi_jmp
SLPolicyInternal.x64=1
SLPolicyOffset.x64=84000
SLPolicyFunc.x64=New_Win8SL

[6.3.9431.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=8A611
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9F721
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=306A8
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=367F9
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2EA25
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=350FD
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=196B0
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=2F9C0
SLInitFunc.x64=New_CSLQuery_Initialize

[6.3.9600.16384]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A2729
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=81824
LocalOnlyCode.x64=nopjmp
SingleUserPatch.x86=1
SingleUserOffset.x86=18028
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=20241
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=16115
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=57829
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=1CEB0
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=554C0
SLInitFunc.x64=New_CSLQuery_Initialize

[6.3.9600.17095]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A36D1
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=B9159
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36BA9
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=21829
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=37529
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1F6A1
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=117F1
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=3B110
SLInitFunc.x64=New_CSLQuery_Initialize

[6.3.9600.17415]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B33F8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8B2D9
LocalOnlyCode.x64=nopjmp
SingleUserPatch.x86=1
SingleUserOffset.x86=37115
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=33CE9
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3CFF9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=45825
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=18478
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=5DBC0
SLInitFunc.x64=New_CSLQuery_Initialize

[6.3.9600.18692]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B3458
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8B2E9
LocalOnlyCode.x64=nopjmp
SingleUserPatch.x86=1
SingleUserOffset.x86=37105
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=37039
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3CFE9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=45835
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=18488
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=5DBD0
SLInitFunc.x64=New_CSLQuery_Initialize

[6.3.9600.18708]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B35D8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8B376
LocalOnlyCode.x64=nopjmp
SingleUserPatch.x86=1
SingleUserOffset.x86=370F5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=36FE9
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3CFD9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=457D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=18308
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=5DB70
SLInitFunc.x64=New_CSLQuery_Initialize

[6.3.9600.18928]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B39D8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8B25D
LocalOnlyCode.x64=nopjmp
SingleUserPatch.x86=1
SingleUserOffset.x86=37D25
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=36C09
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3D6F9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=45495
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=18328
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=5D830
SLInitFunc.x64=New_CSLQuery_Initialize

[6.3.9600.19093]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B3958
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8AE4E
LocalOnlyCode.x64=nopjmp
SingleUserPatch.x86=1
SingleUserOffset.x86=3F045
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=36BC9
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3D899
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=45305
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=18288
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=5D660
SLInitFunc.x64=New_CSLQuery_Initialize

[6.3.9600.19318]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B43E8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=89EAC
LocalOnlyCode.x64=nopjmp
SingleUserPatch.x86=1
SingleUserOffset.x86=3ED25
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=35779
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3D579
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=43CE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=180F8
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=5C0D0
SLInitFunc.x64=New_CSLQuery_Initialize

[6.3.9600.19628]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8A07D
LocalOnlyCode.x64=nopjmp
SingleUserPatch.x64=1
SingleUserOffset.x64=358E9
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=43EF5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=5C2E0
SLInitFunc.x64=New_CSLQuery_Initialize

[6.3.9600.20165]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B3138
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3E5D5
SingleUserCode.x86=nop
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3CE29
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=170A8
SLInitFunc.x86=New_CSLQuery_Initialize
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=889E4
LocalOnlyCode.x64=nopjmp
SingleUserPatch.x64=1
SingleUserOffset.x64=34719
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=42C55
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=5B050
SLInitFunc.x64=New_CSLQuery_Initialize

[6.4.9841.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=956A8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=81141
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=30125
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=12159
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3B989
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=C125
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=46A68
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=1EA50
SLInitFunc.x64=New_CSLQuery_Initialize

[6.4.9860.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=962C8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=81091
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=30845
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=11AA9
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3BEC9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=B9F5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=46F18
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=1EB00
SLInitFunc.x64=New_CSLQuery_Initialize

[6.4.9879.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A9CC8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=95611
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=30C55
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=16A34
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2DAB9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BDC5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=41132
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=24750
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.9926.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8C28
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=31725
SingleUserCode.x86=nop
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3CF99
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=3F140
SLInitFunc.x86=New_CSLQuery_Initialize
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=95FF1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=12A34
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=BE05
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=24EC0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.10041.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A9D88
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97141
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=32215
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=15C64
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2DFC9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=B795
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=46960
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22E40
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.10240.16384]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7D38
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96901
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=32A95
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=18F74
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2F5B9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=22865
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=46581
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=250F0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.10240.18036]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7E18
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96961
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=32715
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17264
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2F299
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=EDC5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=3F968
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=24C30
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.10240.18186]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8048
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96A41
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=32B15
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17264
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2F699
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=EDC5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=3FA58
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=249D0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.10240.18485]
; no x64-version
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8048
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3B6DC
SingleUserCode.x86=nop
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2F699
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=3FA58
SLInitFunc.x86=New_CSLQuery_Initialize

[10.0.10240.18818]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7818
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=95E91
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=395BC
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=18274
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3C629
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=0F0C5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=44677
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=254F0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.10240.19119]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=95F41
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18274
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=0F0C5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=254F0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.10586.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7C18
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96AA1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=353B5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=190D4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=30B69
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=229A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=469DE
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=25220
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.10586.589]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7BE8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96A51
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=353B5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=190D4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=30B69
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=229A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=469DE
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=25220
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.11082.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7C98
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96AB1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35405
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=190D4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=30BB9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=229A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=46A3E
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=25220
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.11102.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A5D58
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=95CD1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35A85
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=2A9C4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=30159
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B5D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=44FD2
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=D160
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14251.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A5D58
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=95CD1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35A85
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=2A9C4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=30159
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B5D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=44FD2
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=D160
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14271.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A4CE8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=941E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35915
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=263F4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF79
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C185
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=47725
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CE50
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14279.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A4D28
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=94191
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35915
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=263F4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF79
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C185
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=47725
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CE50
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14295.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A4D28
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D691
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35925
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=25514
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF89
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BA35
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=47748
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=C860
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14300.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8F5F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=26B04
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1D125
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=CC60
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14316.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8E88
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8F5F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=32B55
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=26B04
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3C1C9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1D295
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=46ABD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CC60
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14328.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8E88
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8F5F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=32B55
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=26B04
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3C1C9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1D365
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=46ABD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CC60
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14332.1001]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8E98
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8F601
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=357E5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=2AE44
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=316A9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C025
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4755F
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CAD0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14342.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8E98
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8EF31
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=357E5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=26774
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=316A9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1CEF5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4755F
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CA20
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14352.1002]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A4478
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D911
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35465
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=24474
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=30099
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1AC05
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=44792
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CDB0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14366.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A9088
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FB01
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=34F65
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=21DE4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=316E9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1A855
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4793E
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CCE0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14367.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A9088
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FB01
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=34F65
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=21DE4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=316E9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1A855
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4793E
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CCE0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14372.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7698
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8F931
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=34635
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=295A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF69
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B295
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=460D2
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CC10
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14379.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7698
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8F941
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=34635
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=295A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF69
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B295
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=460D2
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CC10
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14383.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7698
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8F941
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=34635
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=295A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF69
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B295
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=460D2
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CC10
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14385.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7698
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8F941
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=34635
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=295A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF69
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B295
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=460D2
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CC10
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14388.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6038
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D781
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=359C5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=299A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF29
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1AFC5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45636
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=C930
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14393.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6038
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D781
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=359C5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=299A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF29
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1AFC5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45636
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=C930
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14393.1198]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6088
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=359C5
SingleUserCode.x86=nop
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF29
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=45636
SLInitFunc.x86=New_CSLQuery_Initialize

[10.0.14393.1737]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6198
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D861
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35AD5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=299A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=30039
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1AFC5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45724
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=C930
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14393.2457]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6248
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D811
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36CE5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=29CF4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31209
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B545
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45824
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=C920
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14393.2608]
; no x64 version
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6248
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36CE5
SingleUserCode.x86=nop
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31209
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=45824
SLInitFunc.x86=New_CSLQuery_Initialize

[10.0.14393.2906]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6578
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D8A1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36CE5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1B6A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31209
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=F185
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45912
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22C80
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14393.3383]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6578
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D8A1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36CE5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1B6A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31209
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=F185
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45912
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22C80
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14393.3471]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6528
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D931
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36C65
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1B6A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31189
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=F185
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=458A2
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22C80
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14393.3503]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6528
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D931
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36C65
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1B6A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31189
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=F185
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=458A2
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22C80
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14393.3986]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6578
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D8A1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36CE5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1B6A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31209
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=F185
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45912
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22C80
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14393.4169]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A5B28
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CE51
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=398BC
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=25FA4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3C009
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=29825
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=3F752
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=0CA40
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14393.4704]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CE61
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=23CC8
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=29825
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=0CA40
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14393.4770]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CEE1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=25FA4
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=29825
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=CA40
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14393.5127]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CEF1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=23CC8
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=29825
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=CA40
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14901.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6038
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D781
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=359C5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=299A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF29
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1AFC5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45636
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=C930
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14905.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6038
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D781
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=359C5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=299A4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF29
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1AFC5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45636
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=C930
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14915.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6D98
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8E241
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35E35
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=29EB4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=30399
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B4A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=46092
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CE40
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14926.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A6D18
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8E071
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35E55
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=29EB4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=303B9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B4A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=460A2
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=CE40
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14931.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A4908
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8B411
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35705
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=29264
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FF69
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1AD05
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=452FD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=C7FC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14936.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A3F38
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8B9A1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35355
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=25174
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FCD9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB55
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=44CFE
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=C62C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14942.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A3F38
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9115B
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35355
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=199BD
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FCD9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1064E
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=44CFE
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=258EC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14946.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A4018
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=911AB
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35355
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=199AD
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FCD9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1064E
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=44CFD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=258DC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14951.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A78D8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=94A6B
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3BA85
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1CEDD
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=32629
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=11E9E
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=3F680
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22EE0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14955.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A78D8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=94A6B
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3BA85
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1CEDD
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=32629
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=11E9E
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=3F680
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22EE0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14959.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A79B8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=934AB
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=2EF05
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=16A0D
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2A4E9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=10A8E
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=448A0
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=26960
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14965.1001]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7868
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9345B
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3BA85
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17DFD
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=32A59
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1212E
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=3F680
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=26610
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14971.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7968
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=925FB
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36FE5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1803D
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3D9A9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=11FBE
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=46500
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=26180
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14986.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7878
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=926BB
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36FA5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=17FFD
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3D979
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=11F7E
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=464A0
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=26140
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.14997.1001]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=931EB
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=274ED
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1D95E
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=E000
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15002.1001]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A9698
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=931EB
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=346B5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=274ED
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3D779
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1D95E
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=47D90
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=E000
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15007.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A9648
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=931EB
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=34665
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=274ED
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3D719
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1D95E
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=47D30
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=E000
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15014.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A9648
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=931EB
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=34685
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=274ED
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3D739
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1D95E
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=47D50
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=E000
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15019.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A39F8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=928FB
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=BADF5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=FBDD
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=A8479
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx_jmp
DefPolicyPatch.x64=1
DefPolicyOffset.x64=20AAE
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=3C240
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=24480
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15025.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9259B
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=2C08D
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1DD0E
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=E5B8
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15031.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A5BA8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8E221
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=30A75
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=2A114
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2B1D9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C7B5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4532D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=D80C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15042.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A5BA8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8E221
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=30A75
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=2A114
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2B1D9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C7B5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4532D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=D80C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15046.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=80BB8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8E361
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=31E95
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=15E14
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=38A19
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=E745
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=9422D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=21FFC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15048.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=80BB8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8E361
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=31E95
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=15E14
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=38A19
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=E745
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=9422D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=21FFC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15055.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A5348
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8D2E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=374C5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=181E4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3BAD9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=10B65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=44EFF
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22AEC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15058.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A5D68
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CAA1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35075
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=24E74
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FCD9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=2DD65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4549D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=D1EC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15061.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A5D68
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CAA1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35075
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=24E74
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FCD9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=2DD65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4549D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=D1EC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15063.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A5D68
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CAA1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35075
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=24E74
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FCD9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=2DD65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4549D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=D1EC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15063.296]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A5D68
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CAA1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35075
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=24E74
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=2FCD9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=2DD65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4549D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=D1EC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15063.994]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CB01
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=15EA4
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=FAE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=234DC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15063.1155]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CB01
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=15EA4
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=FAE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=234DC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15063.1746]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A60D8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CB21
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35CA5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=15EA4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=30999
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=FAE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=3F94D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=2328C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.15063.2283]
; no x86-version
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CB21
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=15EA4
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=FAE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2328C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16179.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AA568
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8C141
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=34425
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=16F84
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31219
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1E7F5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45F30
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=21700
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16184.1001]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AA568
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8C141
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=34425
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=16F84
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31219
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1E7F5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45F30
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=21700
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16199.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=ABA68
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8CED1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=348C5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=28C14
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=319B9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=CB25
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=469B0
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=FA30
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16215.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7CE8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8DE21
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39F05
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=28724
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E019
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=CC15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=46462
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=FB00
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16232.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7D38
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8DD41
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39F35
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=287B4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E0C9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=CC15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4650F
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=FB00
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16237.1001]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7F38
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8E911
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39F85
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1BC84
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E119
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=DA55
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4655D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=2180C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16241.1001]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A7F38
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8E911
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39F85
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1BC84
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E119
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=DA55
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4655D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=2180C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16251.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=ABC88
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8EC21
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3A525
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1BCB4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31779
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=DAF5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=447FD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=2183C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16251.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=ABC88
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8EC21
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3A525
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1BCB4
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31779
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=DAF5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=447FD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=2183C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16257.1]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AB718
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8E841
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=33925
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=11364
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3C409
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1EFD5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4504D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=2495C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16257.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AB718
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8E841
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=33925
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=11364
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3C409
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1EFD5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4504D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=2495C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16273.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AB798
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8E871
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=33925
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=11364
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3C409
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1EFD5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4504D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=2495C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16275.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A9388
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=90001
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39435
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1C724
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DE89
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=463D4
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22D0C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16278.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A9388
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=90001
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39435
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1C724
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DE89
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=463D4
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22D0C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16281.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8E08
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FD01
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39215
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1C774
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DC89
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=461BD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22D5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16288.1]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8E08
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FD01
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39215
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1C774
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DC89
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=461BD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22D5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16291.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8E08
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FD01
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39215
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1C774
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DC89
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=461BD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22D5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16294.1]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8E08
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FD01
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39215
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1C774
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DC89
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=461BD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22D5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16296.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8E08
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FD01
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39215
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1C774
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DC89
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=461BD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22D5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16299.0]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8E08
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FD01
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39215
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1C774
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DC89
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=461BD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22D5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16299.15]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8E08
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FD01
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39215
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1C774
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DC89
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=461BD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22D5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16299.1087]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A91F8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FC11
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=392E5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1C774
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DD39
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4626D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22E4C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16353.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A9388
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=90001
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=39435
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1C724
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DE89
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=463D4
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22D0C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.16362.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8E38
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FBA1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=2F61C
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=19D1C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DE99
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=463D4
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22D9C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17004.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=A8EB8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FB41
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=2F65C
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=19D1C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3DF09
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=12D85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=4643F
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22D9C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17017.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AB388
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8F291
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3477C
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1977C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31049
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=125A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45CDD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=227DC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17025.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AB498
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8F291
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3477C
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1977C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31049
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=125A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45CDD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=227DC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17035.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AB3F8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8F271
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=354AC
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=14E7C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31F19
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=10CB5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45C4D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22AEC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17046.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AB3F8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8F281
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=354AC
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=14E8C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=31F19
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=10CC5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=45C4D
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22AFC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17063.1000]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AD7F8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=92671
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36B0C
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=153CC
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=33569
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=111CE
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=474AD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=2318C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17115.1]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AD738
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=925D1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36B0C
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1511C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=33569
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=10E78
DefPolicyCode.x64=CDefPolicy_Query_edi_rcx
SLInitHook.x86=1
SLInitOffset.x86=474AD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22E6C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17128.1]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AD738
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=925D1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36B0C
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1511C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=33569
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=10E78
DefPolicyCode.x64=CDefPolicy_Query_edi_rcx
SLInitHook.x86=1
SLInitOffset.x86=474AD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22E6C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17133.1]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AD738
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=925D1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36B0C
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1511C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=33569
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=10E78
DefPolicyCode.x64=CDefPolicy_Query_edi_rcx
SLInitHook.x86=1
SLInitOffset.x86=474AD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22E6C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17134.1]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AD738
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=925D1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36B0C
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1511C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=33569
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=10E78
DefPolicyCode.x64=CDefPolicy_Query_edi_rcx
SLInitHook.x86=1
SLInitOffset.x86=474AD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22E6C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17134.706]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=ADAB8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=92521
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36B1C
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1511C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=33579
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=10E78
DefPolicyCode.x64=CDefPolicy_Query_edi_rcx
SLInitHook.x86=1
SLInitOffset.x86=475DD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22F5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17134.1304]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=ADAB8
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=92521
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=36B1C
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1511C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=33579
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=10E78
DefPolicyCode.x64=CDefPolicy_Query_edi_rcx
SLInitHook.x86=1
SLInitOffset.x86=475DD
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22F5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17134.1967]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=91BD1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=17CEC
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BC38
DefPolicyCode.x64=CDefPolicy_Query_edi_rcx
SLInitHook.x64=1
SLInitOffset.x64=2328C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17723.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=75D91
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=1296C
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17A45
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1B10C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17738.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=772C1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=124B9
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=179D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1D88C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17746.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=77941
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=132F9
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17F45
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1ABFC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.1]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AF8E4
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=77941
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=4D505
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1322C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4BD09
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17F45
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=5B02A
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=1ABFC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.165]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=77941
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=1322C
; SingleUserOffset.x64=132F9
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17F45
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1ABFC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.168]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AFC74
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=77AF1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=4D665
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1322C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4BE69
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17F45
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=5B18A
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=1ABFC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.288]
; Patch CEnforcementCore::GetInstanceOfTSLicense
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AFAD4
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=77A11
LocalOnlyCode.x64=jmpshort
; Patch CSessionArbitrationHelper::IsSingleSessionPerUserEnabled
SingleUserPatch.x86=1
SingleUserOffset.x86=4D665
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1322C
SingleUserCode.x64=Zero
; Patch CDefPolicy::Query
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4BE69
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17F45
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
; Hook CSLQuery::Initialize
SLInitHook.x86=1
SLInitOffset.x86=5B18A
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=1ABFC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.292]
; Patch CEnforcementCore::GetInstanceOfTSLicense
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AFAD4
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=77A11
LocalOnlyCode.x64=jmpshort
; Patch CSessionArbitrationHelper::IsSingleSessionPerUserEnabled
SingleUserPatch.x86=1
SingleUserOffset.x86=4D665
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1322C
SingleUserCode.x64=Zero
; Patch CDefPolicy::Query
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4BE69
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17F45
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
; Hook CSLQuery::Initialize
SLInitHook.x86=1
SLInitOffset.x86=5B18A
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=1ABFC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.379]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AFAD4
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=77A11
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=4D665
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1322C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4BE69
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17F45
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=5B18A
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=1ABFC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.437]
; Patch CEnforcementCore::GetInstanceOfTSLicense
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AFE24
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=77A41
LocalOnlyCode.x64=jmpshort
; Patch CSessionArbitrationHelper::IsSingleSessionPerUserEnabled
SingleUserPatch.x86=1
SingleUserOffset.x86=4D7B5
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1339C
; SingleUserOffset.x64=1322C
SingleUserCode.x64=Zero
; Patch CDefPolicy::Query
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4BFB9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18025
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
; Hook CSLQuery::Initialize
SLInitHook.x86=1
SLInitOffset.x86=5B2CA
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=1ACDC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.771]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AFEB4
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=4D7F5
SingleUserCode.x86=nop
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4BFF9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=5B30A
SLInitFunc.x86=New_CSLQuery_Initialize
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=77AD1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=1339C
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18025
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1ACDC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.1369]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AFEB4
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=4D7F5
SingleUserCode.x86=nop
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4BFF9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=5B30A
SLInitFunc.x86=New_CSLQuery_Initialize
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=77AD1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13469
; SingleUserOffset.x64=1339C
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18025
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1ACDC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.1613]
LocalOnlyPatch.x86 =1
LocalOnlyOffset.x86 =B5834
LocalOnlyCode.x86 =jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=7E381
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86 =1
SingleUserOffset.x86=4EC35
SingleUserCode.x86 =nop
SingleUserPatch.x64=1
SingleUserOffset.x64=1386C
SingleUserCode.x64=Zero
DefPolicyPatch.x86 =1
DefPolicyOffset.x86 =4D439
DefPolicyCode.x86 =CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=184F5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86 =1
SLInitOffset.x86 =61A0A
SLInitFunc.x86 =New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=2198C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.1697]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B4584
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=7E421
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=4EF55
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=13989
; SingleUserOffset.x64=138BC
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18545
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4D5D9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x64=1
SLInitOffset.x64=21A3C
SLInitFunc.x64=New_CSLQuery_Initialize
SLInitHook.x86=1
SLInitOffset.x86=61C6A
SLInitFunc.x86=New_CSLQuery_Initialize

[10.0.17763.1971]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=77B51
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=134B9
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18075
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1AD9C
SLInitFunc.x64=New_CSLQuery_Initialize
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=AED84
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=4E837
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4CDF9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=5C1DA
SLInitFunc.x86=New_CSLQuery_Initialize

[10.0.17763.2213]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=7E281
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13619
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=181D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2148C
SLInitFunc.x64=New_CSLQuery_Initialize
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B43E4
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=4EDE7
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4D3A9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=6181A
SLInitFunc.x86=New_CSLQuery_Initialize

[10.0.17763.2268]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=7E291
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13879
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18435
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2179C
SLInitFunc.x64=New_CSLQuery_Initialize
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B4384
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=4F007
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4D5C9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=61AAA
SLInitFunc.x86=New_CSLQuery_Initialize

[10.0.17763.2300]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=7E311
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13879
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18435
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2179C
SLInitFunc.x64=New_CSLQuery_Initialize
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B4464
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=4F007
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4D5C9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=61AAA
SLInitFunc.x86=New_CSLQuery_Initialize

[10.0.17763.2628]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=7E7C1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13BF9
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=187B5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=21D3C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.2931]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=7E7C1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13BF9
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=187B5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=21D3C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.2989]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8A541
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=D099
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FFA5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2C29C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.3113]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8A321
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0D099
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FFA5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2C0AC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.17763.3232]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8A5F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0D099
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FFA5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2C29C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.18252.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=780B1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=132B9
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17F05
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1BE4C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.18362.1]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B7A16
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=82F35
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=50515
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=0DBFC
; SingleUserOffset.x64=0DDC9
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=50249
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FE05
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=5A75A
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22DCC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.18362.53]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B7D06
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=82FB5
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=50535
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=0DBFC
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=50269
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FE15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=5A77A
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22DDC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.18362.267]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B7D06
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=82FB5
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=50535
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=0DBFC
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=50269
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FE15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=5A77A
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22DDC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.18362.657]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B7D06
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=82FB5
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=50535
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=0DBFC
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=50269
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FE15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=5A77A
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22DDC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.18362.836]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B7D06
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=82FC5
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=50515
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=0DBFC
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=50249
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FE15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=5A75A
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22DDC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.18362.1316]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B67C6
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=83075
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=35735
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=0DD19
; SingleUserOffset.x64=0DC4C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=4D679
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FE65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=5C18A
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=22E9C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.18362.1533]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=83075
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0DD19
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FE65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22E9C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.18362.1766]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=83075
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0DD19
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FE65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22E9C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.18362.1916]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=830F5
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0DD19
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FE65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22E9C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.18963.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=88C91
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=1A168
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=21C75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2730C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.18362.2158]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=83585
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0DD69
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1FEB5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2309C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=87611
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0BFE2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17ED5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1BDFC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.84]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B46B9
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=87611
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3AD27
SingleUserCode.x86=Zero
SingleUserPatch.x64=1
SingleUserOffset.x64=0BF0C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3D7D9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17ED5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=66658
SLInitFunc.x86=New_CSLQuery_Initialize
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=87611
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0BFE2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17ED5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1BDFC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.662]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B5F59
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=88E81
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3BC05
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=0CAE2
; SingleUserOffset.x64=0CA0C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E779
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=189D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=68068
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=1D50C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.746]
LocalOnlyPatch.x86 =1
LocalOnlyOffset.x86 =B5979
LocalOnlyCode.x86 =jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=88F31
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86 =1
SingleUserOffset.x86=3BC05
SingleUserCode.x86 =nop
SingleUserPatch.x64=1
SingleUserOffset.x64=0CB22
; SingleUserOffset.x64=0CA4C
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18A15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
DefPolicyPatch.x86 =1
DefPolicyOffset.x86 =3E779
DefPolicyCode.x86 =CDefPolicy_Query_eax_ecx
SLInitHook.x64=1
SLInitOffset.x64=1D5BC
SLInitFunc.x64=New_CSLQuery_Initialize
SLInitHook.x86 =1
SLInitOffset.x86 =67B9A
SLInitFunc.x86 =New_CSLQuery_Initialize

[10.0.19041.782]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=88F41
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0CA4C
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18A15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1D5BC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.789]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B59D9
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=88F41
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3BC45
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=0CA4C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E7C9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18A15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=67BF8
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=1D5BC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.962]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=89F31
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0CB22
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18A15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1E29C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.964]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B65C9
LocalOnlyCode.x86=jmpshort
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=89F31
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3BD35
SingleUserCode.x86=nop
SingleUserPatch.x64=1
SingleUserOffset.x64=0CB22
; SingleUserOffset.x64=0CA4C
SingleUserCode.x64=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E8A9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18A15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x86=1
SLInitOffset.x86=687F8
SLInitFunc.x86=New_CSLQuery_Initialize
SLInitHook.x64=1
SLInitOffset.x64=1E29C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1023]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=89C51
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0CB22
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18A15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1DFDC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1081]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=89D81
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0CB26
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=19105
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1E98C
SLInitFunc.x64=New_CSLQuery_Initialize
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B66B9
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3BD25
SingleUserCode.x86=nop
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E899
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=68809
SLInitFunc.x86=New_CSLQuery_Initialize

[10.0.19041.1200]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=89D81
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0D212
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=19105
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1E98C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1202]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B66B9
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3BDE7
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E899
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=68809
SLInitFunc.x86=New_CSLQuery_Initialize
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=89D81
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0D212
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=19105
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1E98C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1319]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=89A21
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0D1E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=190D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1E6AC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1320]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=89A21
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0D1E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=190D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1E6AC
SLInitFunc.x64=New_CSLQuery_Initialize
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B6419
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3BDE7
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E899
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=68578
SLInitFunc.x86=New_CSLQuery_Initialize

[10.0.19041.1348]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=89AC1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0D1E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=190D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1E6AC
SLInitFunc.x64=New_CSLQuery_Initialize
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B64A9
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3BDE7
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E899
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=68578
SLInitFunc.x86=New_CSLQuery_Initialize

[10.0.19041.1379]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8A021
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=D1E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=190D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1E95C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1381]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8A021
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=D1E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=190D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1E95C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1387]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8A021
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0D1E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=190D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1E95C
SLInitFunc.x64=New_CSLQuery_Initialize
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B6899
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3BDE7
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E899
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=68778
SLInitFunc.x86=New_CSLQuery_Initialize

[10.0.19041.1499]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=891F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=D1E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=190D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1DE4C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1503]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B5BD9
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3BB87
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E639
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=67ACA
SLInitFunc.x86=New_CSLQuery_Initialize
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=891F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=D1E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=190D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1DE4C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1561]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B45B9
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3AC17
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3D6C9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=66468
SLInitFunc.x86=New_CSLQuery_Initialize
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=87CD1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=C6E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=185D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1C9AC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1566]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B45B9
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3AC17
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3D6C9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=66468
SLInitFunc.x86=New_CSLQuery_Initialize
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=87CD1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=C6E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=185D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1C9AC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1618]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=877A1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=C6E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=185D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1C72C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1620]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B4219
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3AC17
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3D6C9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=66238
SLInitFunc.x86=New_CSLQuery_Initialize
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=877A1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=C6E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=185D5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1C72C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1679]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=89E21
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=C8C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=187B5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2048C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1682]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=B6839
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3B727
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E1D9
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=68838
SLInitFunc.x86=New_CSLQuery_Initialize
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=89E21
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=C8C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=187B5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2048C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1737]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=941D1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=11902
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1EDC5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2910C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1739]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=941D1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=11902
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1EDC5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2910C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19041.1741]
LocalOnlyPatch.x86=1
LocalOnlyOffset.x86=C4699
LocalOnlyCode.x86=jmpshort
SingleUserPatch.x86=1
SingleUserOffset.x86=3D257
SingleUserCode.x86=Zero
DefPolicyPatch.x86=1
DefPolicyOffset.x86=3E829
DefPolicyCode.x86=CDefPolicy_Query_eax_ecx
SLInitHook.x86=1
SLInitOffset.x86=71298
SLInitFunc.x86=New_CSLQuery_Initialize
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=941D1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=11902
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1EDC5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2910C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19613.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FA01
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13752
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17A85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1AAEC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19619.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FAE6
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13752
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17A85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1AAEC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19628.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FAF1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13742
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17A75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1AB8C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19631.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FCB1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13852
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17B85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
; SLInitOffset.x64=226B0
SLInitOffset.x64=1AE5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19635.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FCB1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13852
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17B85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1AE5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19640.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FCB1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13852
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17B85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1AE5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.19645.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=8FCB1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=13852
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=17B85
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1AE5C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20150.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=95F61
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=16172
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18D25
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1C4AC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20152.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=95F61
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=16172
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18D25
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1C4AC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20161.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96E81
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=160C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18D55
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1D73C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20170.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=974D1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=160D2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18D65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1E28C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20175.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=974D1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=160D2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18D65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1E28C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20180.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=95A11
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=082E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18AB5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1DD1C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20185.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=95A11
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=082E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18AB5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1DD1C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20190.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=95A11
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=082E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18AB5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1DD1C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20197.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=95A31
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=082E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18AB5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1DD3C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20201.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97941
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=8402
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=18BD5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=1F7CC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20206.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97961
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=8972
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B925
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=222AC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20211.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97B51
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=8972
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B925
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=222AC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20215.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97B51
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=8972
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B925
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=222AC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20221.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97B51
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08972
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B925
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=222AC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20226.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97B51
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08972
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B925
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=222AC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20231.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97B51
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08972
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B925
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=222AC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20236.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97B21
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08962
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B915
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2228C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20241.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96EC1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B655
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=21FCC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20246.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96EC1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088E2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B655
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=21FCC
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20251.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96F91
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=089D2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B745
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2237C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20257.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96FD1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=089D2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B745
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2252C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20262.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96FD1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=089D2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B745
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=2252C
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20279.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97171
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=089D2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B745
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22530
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20348.143]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97231
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08A32
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B7A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22600
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20348.261]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97561
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08A32
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B7A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22910
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20348.350]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=975E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08A32
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B7A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22910
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20348.380]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=975E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08A32
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B7A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22910
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20348.502]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97B31
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=8A32
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B7A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22B60
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20348.617]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9A271
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08B32
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B8A5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26790
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20348.681]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9A1A1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08992
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B705
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=268A0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20348.740]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=99AE1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=8992
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B705
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26400
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.20348.859]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=99E61
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=8992
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B705
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26660
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21277.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=96FD1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=089D2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B745
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22530
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21286.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97191
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08612
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B8C5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=226B0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21292.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97251
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08672
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B925
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22780
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21296.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97251
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0859C
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B925
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22780
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21301.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97251
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=0859C
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B925
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22780
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21313.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97371
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08672
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1B925
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22780
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21332.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97511
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08772
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BA25
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=22AD0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21343.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=986F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=25850
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21359.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=986F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=25900
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21370.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=986F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=25900
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21376.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=986F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=25900
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21382.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=986F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=25900
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21387.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=98C11
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26AD0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.21390.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=98C11
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26AD0
SLInitFunc.x64=New_CSLQuery_Initialize

; Windows 11

[10.0.21996.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=98C11
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26AD0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22000.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=98C11
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26AD0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22000.318]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=98CA1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26AD0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22000.466]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=992B1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=88C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26D20
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22000.469]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=992B1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=088C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BB75
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26D20
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22000.652]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=991E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18F22
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BA15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26E50
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22000.653]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=991E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18F22
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BA15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26E50
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22000.708]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=98CB1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18F22
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BA15
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=26C10
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22449.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97DD1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=19152
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BC45
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=270A0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22454.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97DD1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=19152
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BC45
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=270A0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22458.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=97DB1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=19172
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BC65
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=270C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22463.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=99141
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=192C2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BDB5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=27590
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22468.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=99271
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22471.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=99271
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22478.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=992A1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22483.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=992A1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22489.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=992A1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22494.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=992B1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22499.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=993F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22504.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=993F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22509.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=99401
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22518.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=99401
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22523.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=99401
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22526.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=99401
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22533.1001]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=99401
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=193F2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=276C0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22538.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=99601
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=19402
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEF5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=278B0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22543.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=99601
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=19402
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BEF5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=278B0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22557.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9AD11
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08CD2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1BDE5
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=27AA0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22563.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B771
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08CD2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C155
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28620
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22567.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B741
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08CD2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C155
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=285E0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22572.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B631
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=08CD2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C165
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28580
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22579.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B711
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=186B2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C135
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28600
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22581.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B711
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=186B2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C135
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28600
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22593.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B7E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=186B2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C135
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=286D0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22598.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B7E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=186B2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C135
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=286D0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22610.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B7E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=186B2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C135
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=286D0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22616.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B7E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=186B2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C135
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=286D0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22621.1]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B7E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=186B2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C135
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=286D0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22621.317]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B7E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=186B2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C135
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=286D0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.22621.436]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B7E1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=186B2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C135
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=286D0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.25115.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B541
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=186B2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C135
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=286D0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.25120.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B541
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=186B2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C135
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=286D0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.25126.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B561
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=186B2
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C135
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=286D0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.25131.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9BAE1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18D12
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C855
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28DF0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.25136.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9BAE1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18D12
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C855
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28DF0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.25140.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9BC51
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18D12
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C855
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28F60
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.25145.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9BC51
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18D12
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C855
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28F60
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.25151.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9BC51
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18D12
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C855
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28F60
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.25158.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B961
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18D12
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C855
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28F60
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.25163.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B6F1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18D12
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C855
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28EB0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.25169.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B741
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18D12
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C855
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28EB0
SLInitFunc.x64=New_CSLQuery_Initialize

[10.0.25174.1000]
LocalOnlyPatch.x64=1
LocalOnlyOffset.x64=9B7D1
LocalOnlyCode.x64=jmpshort
SingleUserPatch.x64=1
SingleUserOffset.x64=18D12
SingleUserCode.x64=Zero
DefPolicyPatch.x64=1
DefPolicyOffset.x64=1C855
DefPolicyCode.x64=CDefPolicy_Query_eax_rcx
SLInitHook.x64=1
SLInitOffset.x64=28F40
SLInitFunc.x64=New_CSLQuery_Initialize

[SLInit]
bServerSku=1
bRemoteConnAllowed=1
bFUSEnabled=1
bAppServerAllowed=1
bMultimonAllowed=1
lMaxUserSessions=0
ulMaxDebugSessions=0
bInitialized=1

[6.3.9431.0-SLInit]
bFUSEnabled.x86       =A22A8
lMaxUserSessions.x86  =A22AC
bAppServerAllowed.x86 =A22B0
bInitialized.x86      =A22B4
bMultimonAllowed.x86  =A22B8
bServerSku.x86        =A22BC
ulMaxDebugSessions.x86=A22C0
bRemoteConnAllowed.x86=A22C4
bFUSEnabled.x64       =C4490
lMaxUserSessions.x64  =C4494
bAppServerAllowed.x64 =C4498
bInitialized.x64      =C449C
bMultimonAllowed.x64  =C44A0
bServerSku.x64        =C44A4
ulMaxDebugSessions.x64=C44A8
bRemoteConnAllowed.x64=C44AC

[6.3.9600.16384-SLInit]
bFUSEnabled.x86       =C02A8
lMaxUserSessions.x86  =C02AC
bAppServerAllowed.x86 =C02B0
bInitialized.x86      =C02B4
bMultimonAllowed.x86  =C02B8
bServerSku.x86        =C02BC
ulMaxDebugSessions.x86=C02C0
bRemoteConnAllowed.x86=C02C4
bServerSku.x64        =E6494
ulMaxDebugSessions.x64=E6498
bRemoteConnAllowed.x64=E649C
bFUSEnabled.x64       =E64A0
lMaxUserSessions.x64  =E64A4
bAppServerAllowed.x64 =E64A8
bInitialized.x64      =E64AC
bMultimonAllowed.x64  =E64B0

[6.3.9600.17095-SLInit]
bFUSEnabled.x86       =C12A8
lMaxUserSessions.x86  =C12AC
bAppServerAllowed.x86 =C12B0
bInitialized.x86      =C12B4
bMultimonAllowed.x86  =C12B8
bServerSku.x86        =C12BC
ulMaxDebugSessions.x86=C12C0
bRemoteConnAllowed.x86=C12C4
bServerSku.x64        =E4494
ulMaxDebugSessions.x64=E4498
bRemoteConnAllowed.x64=E449C
bFUSEnabled.x64       =E44A0
lMaxUserSessions.x64  =E44A4
bAppServerAllowed.x64 =E44A8
bInitialized.x64      =E44AC
bMultimonAllowed.x64  =E44B0

[6.3.9600.17415-SLInit]
bFUSEnabled.x86       =D3068
lMaxUserSessions.x86  =D306C
bAppServerAllowed.x86 =D3070
bInitialized.x86      =D3074
bMultimonAllowed.x86  =D3078
bServerSku.x86        =D307C
ulMaxDebugSessions.x86=D3080
bRemoteConnAllowed.x86=D3084
bFUSEnabled.x64       =F9054
lMaxUserSessions.x64  =F9058
bAppServerAllowed.x64 =F905C
bInitialized.x64      =F9060
bMultimonAllowed.x64  =F9064
bServerSku.x64        =F9068
ulMaxDebugSessions.x64=F906C
bRemoteConnAllowed.x64=F9070

[6.3.9600.18692-SLInit]
bFUSEnabled.x86       =D3068
lMaxUserSessions.x86  =D306C
bAppServerAllowed.x86 =D3070
bInitialized.x86      =D3074
bMultimonAllowed.x86  =D3078
bServerSku.x86        =D307C
ulMaxDebugSessions.x86=D3080
bRemoteConnAllowed.x86=D3084
bFUSEnabled.x64       =F9054
lMaxUserSessions.x64  =F9058
bAppServerAllowed.x64 =F905C
bInitialized.x64      =F9060
bMultimonAllowed.x64  =F9064
bServerSku.x64        =F9068
ulMaxDebugSessions.x64=F906C
bRemoteConnAllowed.x64=F9070

[6.3.9600.18708-SLInit]
bFUSEnabled.x86       =D3068
lMaxUserSessions.x86  =D306C
bAppServerAllowed.x86 =D3070
bInitialized.x86      =D3074
bMultimonAllowed.x86  =D3078
bServerSku.x86        =D307C
ulMaxDebugSessions.x86=D3080
bRemoteConnAllowed.x86=D3084
bFUSEnabled.x64       =FA054
lMaxUserSessions.x64  =FA058
bAppServerAllowed.x64 =FA05C
bInitialized.x64      =FA060
bMultimonAllowed.x64  =FA064
bServerSku.x64        =FA068
ulMaxDebugSessions.x64=FA06C
bRemoteConnAllowed.x64=FA070

[6.3.9600.18928-SLInit]
bFUSEnabled.x86       =D3068
lMaxUserSessions.x86  =D306C
bAppServerAllowed.x86 =D3070
bInitialized.x86      =D3074
bMultimonAllowed.x86  =D3078
bServerSku.x86        =D307C
ulMaxDebugSessions.x86=D3080
bRemoteConnAllowed.x86=D3084
bFUSEnabled.x64       =FA054
lMaxUserSessions.x64  =FA058
bAppServerAllowed.x64 =FA05C
bInitialized.x64      =FA060
bMultimonAllowed.x64  =FA064
bServerSku.x64        =FA068
ulMaxDebugSessions.x64=FA06C
bRemoteConnAllowed.x64=FA070

[6.3.9600.19093-SLInit]
bFUSEnabled.x86       =D3068
lMaxUserSessions.x86  =D306C
bAppServerAllowed.x86 =D3070
bInitialized.x86      =D3074
bMultimonAllowed.x86  =D3078
bServerSku.x86        =D307C
ulMaxDebugSessions.x86=D3080
bRemoteConnAllowed.x86=D3084
bFUSEnabled.x64       =FA054
lMaxUserSessions.x64  =FA058
bAppServerAllowed.x64 =FA05C
bInitialized.x64      =FA060
bMultimonAllowed.x64  =FA064
bServerSku.x64        =FA068
ulMaxDebugSessions.x64=FA06C
bRemoteConnAllowed.x64=FA070

[6.3.9600.19318-SLInit]
bFUSEnabled.x86       =D4068
lMaxUserSessions.x86  =D406C
bAppServerAllowed.x86 =D4070
bInitialized.x86      =D4074
bMultimonAllowed.x86  =D4078
bServerSku.x86        =D407C
ulMaxDebugSessions.x86=D4080
bRemoteConnAllowed.x86=D4084
bFUSEnabled.x64       =FA054
lMaxUserSessions.x64  =FA058
bAppServerAllowed.x64 =FA05C
bInitialized.x64      =FA060
bMultimonAllowed.x64  =FA064
bServerSku.x64        =FA068
ulMaxDebugSessions.x64=FA06C
bRemoteConnAllowed.x64=FA070

[6.3.9600.19628-SLInit]
bFUSEnabled.x64       =FA054
lMaxUserSessions.x64  =FA058
bAppServerAllowed.x64 =FA05C
bInitialized.x64      =FA060
bMultimonAllowed.x64  =FA064
bServerSku.x64        =FA068
ulMaxDebugSessions.x64=FA06C
bRemoteConnAllowed.x64=FA070

[6.3.9600.20165-SLInit]
bFUSEnabled.x86       =D2068
lMaxUserSessions.x86  =D206C
bAppServerAllowed.x86 =D2070
bInitialized.x86      =D2074
bMultimonAllowed.x86  =D2078
bServerSku.x86        =D207C
ulMaxDebugSessions.x86=D2080
bRemoteConnAllowed.x86=D2084
bFUSEnabled.x64       =F8054
lMaxUserSessions.x64  =F8058
bAppServerAllowed.x64 =F805C
bInitialized.x64      =F8060
bMultimonAllowed.x64  =F8064
bServerSku.x64        =F8068
ulMaxDebugSessions.x64=F806C
bRemoteConnAllowed.x64=F8070

[6.4.9841.0-SLInit]
bFUSEnabled.x86       =BF9F0
lMaxUserSessions.x86  =BF9F4
bAppServerAllowed.x86 =BF9F8
bInitialized.x86      =BF9FC
bMultimonAllowed.x86  =BFA00
bServerSku.x86        =BFA04
ulMaxDebugSessions.x86=BFA08
bRemoteConnAllowed.x86=BFA0C
bFUSEnabled.x64       =ECFF8
lMaxUserSessions.x64  =ECFFC
bAppServerAllowed.x64 =ED000
bInitialized.x64      =ED004
bMultimonAllowed.x64  =ED008
bServerSku.x64        =ED00C
ulMaxDebugSessions.x64=ED010
bRemoteConnAllowed.x64=ED014

[6.4.9860.0-SLInit]
bFUSEnabled.x86       =BF7E0
lMaxUserSessions.x86  =BF7E4
bAppServerAllowed.x86 =BF7E8
bInitialized.x86      =BF7EC
bMultimonAllowed.x86  =BF7F0
bServerSku.x86        =BF7F4
ulMaxDebugSessions.x86=BF7F8
bRemoteConnAllowed.x86=BF7FC
bFUSEnabled.x64       =ECBD8
lMaxUserSessions.x64  =ECBDC
bAppServerAllowed.x64 =ECBE0
bInitialized.x64      =ECBE4
bMultimonAllowed.x64  =ECBE8
bServerSku.x64        =ECBEC
ulMaxDebugSessions.x64=ECBF0
bRemoteConnAllowed.x64=ECBF4

[6.4.9879.0-SLInit]
bFUSEnabled.x86       =C27D8
lMaxUserSessions.x86  =C27DC
bAppServerAllowed.x86 =C27E0
bInitialized.x86      =C27E4
bMultimonAllowed.x86  =C27E8
bServerSku.x86        =C27EC
ulMaxDebugSessions.x86=C27F0
bRemoteConnAllowed.x86=C27F4
bFUSEnabled.x64       =EDBF0
lMaxUserSessions.x64  =EDBF4
bAppServerAllowed.x64 =EDBF8
bInitialized.x64      =EDBFC
bMultimonAllowed.x64  =EDC00
bServerSku.x64        =EDC04
ulMaxDebugSessions.x64=EDC08
bRemoteConnAllowed.x64=EDC0C

[10.0.9926.0-SLInit]
bFUSEnabled.x86       =C17D8
lMaxUserSessions.x86  =C17DC
bAppServerAllowed.x86 =C17E0
bInitialized.x86      =C17E4
bMultimonAllowed.x86  =C17E8
bServerSku.x86        =C17EC
ulMaxDebugSessions.x86=C17F0
bRemoteConnAllowed.x86=C17F4
bFUSEnabled.x64       =EEBF0
lMaxUserSessions.x64  =EEBF4
bAppServerAllowed.x64 =EEBF8
bInitialized.x64      =EEBFC
bMultimonAllowed.x64  =EEC00
bServerSku.x64        =EEC04
ulMaxDebugSessions.x64=EEC08
bRemoteConnAllowed.x64=EEC0C

[10.0.10041.0-SLInit]
bFUSEnabled.x86       =C5F60
lMaxUserSessions.x86  =C5F64
bAppServerAllowed.x86 =C5F68
bInitialized.x86      =C5F6C
bMultimonAllowed.x86  =C5F70
bServerSku.x86        =C5F74
ulMaxDebugSessions.x86=C5F78
bRemoteConnAllowed.x86=C5F7C
bFUSEnabled.x64       =F3448
lMaxUserSessions.x64  =F344C
bAppServerAllowed.x64 =F3450
bInitialized.x64      =F3454
bMultimonAllowed.x64  =F3458
bServerSku.x64        =F345C
ulMaxDebugSessions.x64=F3460
bRemoteConnAllowed.x64=F3464

[10.0.10240.16384-SLInit]
bFUSEnabled.x86       =C3F60
lMaxUserSessions.x86  =C3F64
bAppServerAllowed.x86 =C3F68
bInitialized.x86      =C3F6C
bMultimonAllowed.x86  =C3F70
bServerSku.x86        =C3F74
ulMaxDebugSessions.x86=C3F78
bRemoteConnAllowed.x86=C3F7C
zlMaxUserSessions.x64 =F23B0
lMaxUserSessions.x64  =F23B0
bAppServerAllowed.x64 =F23B4
bServerSku.x64        =F23B8
bFUSEnabled.x64       =F3460
bInitialized.x64      =F3464
bMultimonAllowed.x64  =F3468
ulMaxDebugSessions.x64=F346C
bRemoteConnAllowed.x64=F3470

[10.0.10240.18036-SLInit]
bFUSEnabled.x86       =C3F88
lMaxUserSessions.x86  =C3F8C
bAppServerAllowed.x86 =C3F90
bInitialized.x86      =C3F94
bMultimonAllowed.x86  =C3F98
bServerSku.x86        =C3F9C
ulMaxDebugSessions.x86=C3FA0
bRemoteConnAllowed.x86=C3FA4
lMaxUserSessions.x64  =F23B0
bAppServerAllowed.x64 =F23B4
bServerSku.x64        =F23B8
bFUSEnabled.x64       =F3460
bInitialized.x64      =F3464
bMultimonAllowed.x64  =F3468
ulMaxDebugSessions.x64=F346C
bRemoteConnAllowed.x64=F3470

[10.0.10240.18186-SLInit]
bFUSEnabled.x86       =C4F88
lMaxUserSessions.x86  =C4F8C
bAppServerAllowed.x86 =C4F90
bInitialized.x86      =C4F94
bMultimonAllowed.x86  =C4F98
bServerSku.x86        =C4F9C
ulMaxDebugSessions.x86=C4FA0
bRemoteConnAllowed.x86=C4FA4
lMaxUserSessions.x64  =F23B0
bAppServerAllowed.x64 =F23B4
bServerSku.x64        =F23B8
bFUSEnabled.x64       =F3460
bInitialized.x64      =F3464
bMultimonAllowed.x64  =F3468
ulMaxDebugSessions.x64=F346C
bRemoteConnAllowed.x64=F3470

[10.0.10240.18485-SLInit]
; no x64-version
bFUSEnabled.x86       =C4F88
lMaxUserSessions.x86  =C4F8C
bAppServerAllowed.x86 =C4F90
bInitialized.x86      =C4F94
bMultimonAllowed.x86  =C4F98
bServerSku.x86        =C4F9C
ulMaxDebugSessions.x86=C4FA0
bRemoteConnAllowed.x86=C4FA4

[10.0.10240.18818-SLInit]
bInitialized.x86      =C3F94
bServerSku.x86        =C3F9C
lMaxUserSessions.x86  =C3F8C
bAppServerAllowed.x86 =C3F90
bRemoteConnAllowed.x86=C3FA4
bMultimonAllowed.x86  =C3F98
ulMaxDebugSessions.x86=C3FA0
bFUSEnabled.x86       =C3F88
lMaxUserSessions.x64  =F13B0
bAppServerAllowed.x64 =F13B4
bServerSku.x64        =F13B8
bFUSEnabled.x64       =F2460
bInitialized.x64      =F2464
bMultimonAllowed.x64  =F2468
ulMaxDebugSessions.x64=F246C
bRemoteConnAllowed.x64=F2470

[10.0.10240.19119-SLInit]
bInitialized.x64      =F2464
bServerSku.x64        =F13B8
lMaxUserSessions.x64  =F13B0
bAppServerAllowed.x64 =F13B4
bRemoteConnAllowed.x64=F2470
bMultimonAllowed.x64  =F2468
ulMaxDebugSessions.x64=F246C
bFUSEnabled.x64       =F2470

[10.0.10586.0-SLInit]
bFUSEnabled.x86       =C3F60
lMaxUserSessions.x86  =C3F64
bAppServerAllowed.x86 =C3F68
bInitialized.x86      =C3F6C
bMultimonAllowed.x86  =C3F70
bServerSku.x86        =C3F74
ulMaxDebugSessions.x86=C3F78
bRemoteConnAllowed.x86=C3F7C
lMaxUserSessions.x64  =F23B0
bAppServerAllowed.x64 =F23B4
bServerSku.x64        =F23B8
bFUSEnabled.x64       =F3460
bInitialized.x64      =F3464
bMultimonAllowed.x64  =F3468
ulMaxDebugSessions.x64=F346C
bRemoteConnAllowed.x64=F3470

[10.0.10586.589-SLInit]
bFUSEnabled.x86       =C3F60
lMaxUserSessions.x86  =C3F64
bAppServerAllowed.x86 =C3F68
bInitialized.x86      =C3F6C
bMultimonAllowed.x86  =C3F70
bServerSku.x86        =C3F74
ulMaxDebugSessions.x86=C3F78
bRemoteConnAllowed.x86=C3F7C
lMaxUserSessions.x64  =F23B0
bAppServerAllowed.x64 =F23B4
bServerSku.x64        =F23B8
bFUSEnabled.x64       =F3460
bInitialized.x64      =F3464
bMultimonAllowed.x64  =F3468
ulMaxDebugSessions.x64=F346C
bRemoteConnAllowed.x64=F3470

[10.0.11082.1000-SLInit]
bFUSEnabled.x86       =C3F60
lMaxUserSessions.x86  =C3F64
bAppServerAllowed.x86 =C3F68
bInitialized.x86      =C3F6C
bMultimonAllowed.x86  =C3F70
bServerSku.x86        =C3F74
ulMaxDebugSessions.x86=C3F78
bRemoteConnAllowed.x86=C3F7C
lMaxUserSessions.x64  =F23B0
bAppServerAllowed.x64 =F23B4
bServerSku.x64        =F23B8
bFUSEnabled.x64       =F3460
bInitialized.x64      =F3464
bMultimonAllowed.x64  =F3468
ulMaxDebugSessions.x64=F346C
bRemoteConnAllowed.x64=F3470

[10.0.11102.1000-SLInit]
bInitialized.x86      =C1F5C
bServerSku.x86        =C1F60
lMaxUserSessions.x86  =C1F64
bAppServerAllowed.x86 =C1F68
bRemoteConnAllowed.x86=C1F6C
bMultimonAllowed.x86  =C1F70
ulMaxDebugSessions.x86=C1F74
bFUSEnabled.x86       =C1F78
bInitialized.x64      =F2430
bRemoteConnAllowed.x64=F2434
bMultimonAllowed.x64  =F2438
ulMaxDebugSessions.x64=F243C
bFUSEnabled.x64       =F2440
bServerSku.x64        =F244C
lMaxUserSessions.x64  =F2450
bAppServerAllowed.x64 =F2454

[10.0.14251.1000-SLInit]
bInitialized.x86      =C1F5C
bServerSku.x86        =C1F60
lMaxUserSessions.x86  =C1F64
bAppServerAllowed.x86 =C1F68
bRemoteConnAllowed.x86=C1F6C
bMultimonAllowed.x86  =C1F70
ulMaxDebugSessions.x86=C1F74
bFUSEnabled.x86       =C1F78
bInitialized.x64      =F2430
bRemoteConnAllowed.x64=F2434
bMultimonAllowed.x64  =F2438
ulMaxDebugSessions.x64=F243C
bFUSEnabled.x64       =F2440
bServerSku.x64        =F244C
lMaxUserSessions.x64  =F2450
bAppServerAllowed.x64 =F2454

[10.0.14271.1000-SLInit]
bInitialized.x86      =C0F5C
bServerSku.x86        =C0F60
lMaxUserSessions.x86  =C0F64
bAppServerAllowed.x86 =C0F68
bRemoteConnAllowed.x86=C0F6C
bMultimonAllowed.x86  =C0F70
ulMaxDebugSessions.x86=C0F74
bFUSEnabled.x86       =C0F78
bServerSku.x64        =EF3C0
lMaxUserSessions.x64  =EF3C4
bAppServerAllowed.x64 =EF3C8
bInitialized.x64      =F0460
bRemoteConnAllowed.x64=F0464
bMultimonAllowed.x64  =F0468
ulMaxDebugSessions.x64=F046C
bFUSEnabled.x64       =F0470

[10.0.14279.1000-SLInit]
bInitialized.x86      =C0F5C
bServerSku.x86        =C0F60
lMaxUserSessions.x86  =C0F64
bAppServerAllowed.x86 =C0F68
bRemoteConnAllowed.x86=C0F6C
bMultimonAllowed.x86  =C0F70
ulMaxDebugSessions.x86=C0F74
bFUSEnabled.x86       =C0F78
bServerSku.x64        =EF3C0
lMaxUserSessions.x64  =EF3C4
bAppServerAllowed.x64 =EF3C8
bInitialized.x64      =F0460
bRemoteConnAllowed.x64=F0464
bMultimonAllowed.x64  =F0468
ulMaxDebugSessions.x64=F046C
bFUSEnabled.x64       =F0470

[10.0.14295.1000-SLInit]
bInitialized.x86      =C0F5C
bServerSku.x86        =C0F60
lMaxUserSessions.x86  =C0F64
bAppServerAllowed.x86 =C0F68
bRemoteConnAllowed.x86=C0F6C
bMultimonAllowed.x86  =C0F70
ulMaxDebugSessions.x86=C0F74
bFUSEnabled.x86       =C0F78
bServerSku.x64        =E73C0
lMaxUserSessions.x64  =E73C4
bAppServerAllowed.x64 =E73C8
bInitialized.x64      =E8460
bRemoteConnAllowed.x64=E8464
bMultimonAllowed.x64  =E8468
ulMaxDebugSessions.x64=E846C
bFUSEnabled.x64       =E8470

[10.0.14300.1000-SLInit]
bServerSku.x64        =E93C0
lMaxUserSessions.x64  =E93C4
bAppServerAllowed.x64 =E93C8
bInitialized.x64      =EA460
bRemoteConnAllowed.x64=EA464
bMultimonAllowed.x64  =EA468
ulMaxDebugSessions.x64=EA46C
bFUSEnabled.x64       =EA470

[10.0.14316.1000-SLInit]
bInitialized.x86      =C4F58
bServerSku.x86        =C4F5C
lMaxUserSessions.x86  =C4F60
bAppServerAllowed.x86 =C4F64
bRemoteConnAllowed.x86=C4F68
bMultimonAllowed.x86  =C4F6C
ulMaxDebugSessions.x86=C4F70
bFUSEnabled.x86       =C4F74
bServerSku.x64        =E93C0
lMaxUserSessions.x64  =E93C4
bAppServerAllowed.x64 =E93C8
bInitialized.x64      =EA460
bRemoteConnAllowed.x64=EA464
bMultimonAllowed.x64  =EA468
ulMaxDebugSessions.x64=EA46C
bFUSEnabled.x64       =EA470

[10.0.14328.1000-SLInit]
bInitialized.x86      =C4F58
bServerSku.x86        =C4F5C
lMaxUserSessions.x86  =C4F60
bAppServerAllowed.x86 =C4F64
bRemoteConnAllowed.x86=C4F68
bMultimonAllowed.x86  =C4F6C
ulMaxDebugSessions.x86=C4F70
bFUSEnabled.x86       =C4F74
bServerSku.x64        =E93C0
lMaxUserSessions.x64  =E93C4
bAppServerAllowed.x64 =E93C8
bInitialized.x64      =EA460
bRemoteConnAllowed.x64=EA464
bMultimonAllowed.x64  =EA468
ulMaxDebugSessions.x64=EA46C
bFUSEnabled.x64       =EA470

[10.0.14332.1001-SLInit]
bInitialized.x86      =C4F58
bServerSku.x86        =C4F5C
lMaxUserSessions.x86  =C4F60
bAppServerAllowed.x86 =C4F64
bRemoteConnAllowed.x86=C4F68
bMultimonAllowed.x86  =C4F6C
ulMaxDebugSessions.x86=C4F70
bFUSEnabled.x86       =C4F74
bServerSku.x64        =E93C0
lMaxUserSessions.x64  =E93C4
bAppServerAllowed.x64 =E93C8
bInitialized.x64      =EA460
bRemoteConnAllowed.x64=EA464
bMultimonAllowed.x64  =EA468
ulMaxDebugSessions.x64=EA46C
bFUSEnabled.x64       =EA470

[10.0.14342.1000-SLInit]
bInitialized.x86      =C4F58
bServerSku.x86        =C4F5C
lMaxUserSessions.x86  =C4F60
bAppServerAllowed.x86 =C4F64
bRemoteConnAllowed.x86=C4F68
bMultimonAllowed.x86  =C4F6C
ulMaxDebugSessions.x86=C4F70
bFUSEnabled.x86       =C4F74
bInitialized.x64      =E9430
bRemoteConnAllowed.x64=E9434
bMultimonAllowed.x64  =E9438
ulMaxDebugSessions.x64=E943C
bFUSEnabled.x64       =E9440
bServerSku.x64        =E944C
lMaxUserSessions.x64  =E9450
bAppServerAllowed.x64 =E9454

[10.0.14352.1002-SLInit]
bInitialized.x86      =C0F5C
bServerSku.x86        =C0F60
lMaxUserSessions.x86  =C0F64
bAppServerAllowed.x86 =C0F68
bRemoteConnAllowed.x86=C0F6C
bMultimonAllowed.x86  =C0F70
ulMaxDebugSessions.x86=C0F74
bFUSEnabled.x86       =C0F78
bServerSku.x64        =E73C0
lMaxUserSessions.x64  =E73C4
bAppServerAllowed.x64 =E73C8
bInitialized.x64      =E8460
bRemoteConnAllowed.x64=E8464
bMultimonAllowed.x64  =E8468
ulMaxDebugSessions.x64=E846C
bFUSEnabled.x64       =E8470

[10.0.14366.0-SLInit]
bInitialized.x86      =C4F68
bServerSku.x86        =C4F6C
lMaxUserSessions.x86  =C4F70
bAppServerAllowed.x86 =C4F74
bRemoteConnAllowed.x86=C4F78
bMultimonAllowed.x86  =C4F7C
ulMaxDebugSessions.x86=C4F80
bFUSEnabled.x86       =C4F84
bServerSku.x64        =E93E0
lMaxUserSessions.x64  =E93E4
bAppServerAllowed.x64 =E93E8
bInitialized.x64      =EA480
bRemoteConnAllowed.x64=EA484
bMultimonAllowed.x64  =EA488
ulMaxDebugSessions.x64=EA48C
bFUSEnabled.x64       =EA490

[10.0.14367.0-SLInit]
bInitialized.x86      =C4F68
bServerSku.x86        =C4F6C
lMaxUserSessions.x86  =C4F70
bAppServerAllowed.x86 =C4F74
bRemoteConnAllowed.x86=C4F78
bMultimonAllowed.x86  =C4F7C
ulMaxDebugSessions.x86=C4F80
bFUSEnabled.x86       =C4F84
bServerSku.x64        =E93E0
lMaxUserSessions.x64  =E93E4
bAppServerAllowed.x64 =E93E8
bInitialized.x64      =EA480
bRemoteConnAllowed.x64=EA484
bMultimonAllowed.x64  =EA488
ulMaxDebugSessions.x64=EA48C
bFUSEnabled.x64       =EA490

[10.0.14372.0-SLInit]
bInitialized.x86      =C3F68
bServerSku.x86        =C3F6C
lMaxUserSessions.x86  =C3F70
bAppServerAllowed.x86 =C3F74
bRemoteConnAllowed.x86=C3F78
bMultimonAllowed.x86  =C3F7C
ulMaxDebugSessions.x86=C3F80
bFUSEnabled.x86       =C3F84
bInitialized.x64      =EA460
bRemoteConnAllowed.x64=EA464
bMultimonAllowed.x64  =EA468
ulMaxDebugSessions.x64=EA46C
bFUSEnabled.x64       =EA470
bServerSku.x64        =EA47C
lMaxUserSessions.x64  =EA480
bAppServerAllowed.x64 =EA484

[10.0.14379.0-SLInit]
bInitialized.x86      =C3F68
bServerSku.x86        =C3F6C
lMaxUserSessions.x86  =C3F70
bAppServerAllowed.x86 =C3F74
bRemoteConnAllowed.x86=C3F78
bMultimonAllowed.x86  =C3F7C
ulMaxDebugSessions.x86=C3F80
bFUSEnabled.x86       =C3F84
bInitialized.x64      =EA460
bRemoteConnAllowed.x64=EA464
bMultimonAllowed.x64  =EA468
ulMaxDebugSessions.x64=EA46C
bFUSEnabled.x64       =EA470
bServerSku.x64        =EA47C
lMaxUserSessions.x64  =EA480
bAppServerAllowed.x64 =EA484

[10.0.14383.0-SLInit]
bInitialized.x86      =C3F68
bServerSku.x86        =C3F6C
lMaxUserSessions.x86  =C3F70
bAppServerAllowed.x86 =C3F74
bRemoteConnAllowed.x86=C3F78
bMultimonAllowed.x86  =C3F7C
ulMaxDebugSessions.x86=C3F80
bFUSEnabled.x86       =C3F84
bInitialized.x64      =EA460
bRemoteConnAllowed.x64=EA464
bMultimonAllowed.x64  =EA468
ulMaxDebugSessions.x64=EA46C
bFUSEnabled.x64       =EA470
bServerSku.x64        =EA47C
lMaxUserSessions.x64  =EA480
bAppServerAllowed.x64 =EA484

[10.0.14385.0-SLInit]
bInitialized.x86      =C3F68
bServerSku.x86        =C3F6C
lMaxUserSessions.x86  =C3F70
bAppServerAllowed.x86 =C3F74
bRemoteConnAllowed.x86=C3F78
bMultimonAllowed.x86  =C3F7C
ulMaxDebugSessions.x86=C3F80
bFUSEnabled.x86       =C3F84
bInitialized.x64      =EA460
bRemoteConnAllowed.x64=EA464
bMultimonAllowed.x64  =EA468
ulMaxDebugSessions.x64=EA46C
bFUSEnabled.x64       =EA470
bServerSku.x64        =EA47C
lMaxUserSessions.x64  =EA480
bAppServerAllowed.x64 =EA484

[10.0.14388.0-SLInit]
bInitialized.x86      =C1F6C
bServerSku.x86        =C1F70
lMaxUserSessions.x86  =C1F74
bAppServerAllowed.x86 =C1F78
bRemoteConnAllowed.x86=C1F7C
bMultimonAllowed.x86  =C1F80
ulMaxDebugSessions.x86=C1F84
bFUSEnabled.x86       =C1F88
bServerSku.x64        =E73D0
lMaxUserSessions.x64  =E73D4
bAppServerAllowed.x64 =E73D8
bInitialized.x64      =E8470
bRemoteConnAllowed.x64=E8474
bMultimonAllowed.x64  =E8478
ulMaxDebugSessions.x64=E847C
bFUSEnabled.x64       =E8480

[10.0.14393.0-SLInit]
bInitialized.x86      =C1F6C
bServerSku.x86        =C1F70
lMaxUserSessions.x86  =C1F74
bAppServerAllowed.x86 =C1F78
bRemoteConnAllowed.x86=C1F7C
bMultimonAllowed.x86  =C1F80
ulMaxDebugSessions.x86=C1F84
bFUSEnabled.x86       =C1F88
bServerSku.x64        =E73D0
lMaxUserSessions.x64  =E73D4
bAppServerAllowed.x64 =E73D8
bInitialized.x64      =E8470
bRemoteConnAllowed.x64=E8474
bMultimonAllowed.x64  =E8478
ulMaxDebugSessions.x64=E847C
bFUSEnabled.x64       =E8480

[10.0.14393.1198-SLInit]
bInitialized.x86      =C1F6C
bServerSku.x86        =C1F70
lMaxUserSessions.x86  =C1F74
bAppServerAllowed.x86 =C1F78
bRemoteConnAllowed.x86=C1F7C
bMultimonAllowed.x86  =C1F80
ulMaxDebugSessions.x86=C1F84
bFUSEnabled.x86       =C1F88

[10.0.14393.1737-SLInit]
bInitialized.x86      =C1F6C
bServerSku.x86        =C1F70
lMaxUserSessions.x86  =C1F74
bAppServerAllowed.x86 =C1F78
bRemoteConnAllowed.x86=C1F7C
bMultimonAllowed.x86  =C1F80
ulMaxDebugSessions.x86=C1F84
bFUSEnabled.x86       =C1F88
bServerSku.x64        =E73D0
lMaxUserSessions.x64  =E73D4
bAppServerAllowed.x64 =E73D8
bInitialized.x64      =E8470
bRemoteConnAllowed.x64=E8474
bMultimonAllowed.x64  =E8478
ulMaxDebugSessions.x64=E847C
bFUSEnabled.x64       =E8480

[10.0.14393.2457-SLInit]
bInitialized.x86      =C1F94
bServerSku.x86        =C1F98
lMaxUserSessions.x86  =C1F9C
bAppServerAllowed.x86 =C1FA0
bRemoteConnAllowed.x86=C1FA4
bMultimonAllowed.x86  =C1FA8
ulMaxDebugSessions.x86=C1FAC
bFUSEnabled.x86       =C1FB0
bServerSku.x64        =E73D0
lMaxUserSessions.x64  =E73D4
bAppServerAllowed.x64 =E73D8
bInitialized.x64      =E8470
bRemoteConnAllowed.x64=E8474
bMultimonAllowed.x64  =E8478
ulMaxDebugSessions.x64=E847C
bFUSEnabled.x64       =E8480

[10.0.14393.2608-SLInit]
; no x64 version
bInitialized.x86      =C1F94
bServerSku.x86        =C1F98
lMaxUserSessions.x86  =C1F9C
bAppServerAllowed.x86 =C1FA0
bRemoteConnAllowed.x86=C1FA4
bMultimonAllowed.x86  =C1FA8
ulMaxDebugSessions.x86=C1FAC
bFUSEnabled.x86       =C1FB0

[10.0.14393.2906-SLInit]
bInitialized.x86      =C2F94
bServerSku.x86        =C2F98
lMaxUserSessions.x86  =C2F9C
bAppServerAllowed.x86 =C2FA0
bRemoteConnAllowed.x86=C2FA4
bMultimonAllowed.x86  =C2FA8
ulMaxDebugSessions.x86=C2FAC
bFUSEnabled.x86       =C2FB0
bServerSku.x64        =E73D0
lMaxUserSessions.x64  =E73D4
bAppServerAllowed.x64 =E73D8
bInitialized.x64      =E8470
bRemoteConnAllowed.x64=E8474
bMultimonAllowed.x64  =E8478
ulMaxDebugSessions.x64=E847C
bFUSEnabled.x64       =E8480

[10.0.14393.3383-SLInit]
bInitialized.x86      =C2F94
bServerSku.x86        =C2F98
lMaxUserSessions.x86  =C2F9C
bAppServerAllowed.x86 =C2FA0
bRemoteConnAllowed.x86=C2FA4
bMultimonAllowed.x86  =C2FA8
ulMaxDebugSessions.x86=C2FAC
bFUSEnabled.x86       =C2FB0
bServerSku.x64        =E73D0
lMaxUserSessions.x64  =E73D4
bAppServerAllowed.x64 =E73D8
bInitialized.x64      =E8470
bRemoteConnAllowed.x64=E8474
bMultimonAllowed.x64  =E8478
ulMaxDebugSessions.x64=E847C
bFUSEnabled.x64       =E8480

[10.0.14393.3471-SLInit]
bInitialized.x86      =C2F94
bServerSku.x86        =C2F98
lMaxUserSessions.x86  =C2F9C
bAppServerAllowed.x86 =C2FA0
bRemoteConnAllowed.x86=C2FA4
bMultimonAllowed.x86  =C2FA8
ulMaxDebugSessions.x86=C2FAC
bFUSEnabled.x86       =C2FB0
bServerSku.x64        =E73D0
lMaxUserSessions.x64  =E73D4
bAppServerAllowed.x64 =E73D8
bInitialized.x64      =E8470
bRemoteConnAllowed.x64=E8474
bMultimonAllowed.x64  =E8478
ulMaxDebugSessions.x64=E847C
bFUSEnabled.x64       =E8480

[10.0.14393.3503-SLInit]
bInitialized.x86      =C2F94
bServerSku.x86        =C2F98
lMaxUserSessions.x86  =C2F9C
bAppServerAllowed.x86 =C2FA0
bRemoteConnAllowed.x86=C2FA4
bMultimonAllowed.x86  =C2FA8
ulMaxDebugSessions.x86=C2FAC
bFUSEnabled.x86       =C2FB0
bServerSku.x64        =E73D0
lMaxUserSessions.x64  =E73D4
bAppServerAllowed.x64 =E73D8
bInitialized.x64      =E8470
bRemoteConnAllowed.x64=E8474
bMultimonAllowed.x64  =E8478
ulMaxDebugSessions.x64=E847C
bFUSEnabled.x64       =E8480

[10.0.14393.3986-SLInit]
bInitialized.x86      =C2F94
bServerSku.x86        =C2F98
lMaxUserSessions.x86  =C2F9C
bAppServerAllowed.x86 =C2FA0
bRemoteConnAllowed.x86=C2FA4
bMultimonAllowed.x86  =C2FA8
ulMaxDebugSessions.x86=C2FAC
bFUSEnabled.x86       =C2FB0
bServerSku.x64        =E73D0
lMaxUserSessions.x64  =E73D4
bAppServerAllowed.x64 =E73D8
bInitialized.x64      =E8470
bRemoteConnAllowed.x64=E8474
bMultimonAllowed.x64  =E8478
ulMaxDebugSessions.x64=E847C
bFUSEnabled.x64       =E8480

[10.0.14393.4169-SLInit]
bInitialized.x86      =C1F94
bServerSku.x86        =C1F98
lMaxUserSessions.x86  =C1F9C
bAppServerAllowed.x86 =C1FA0
bRemoteConnAllowed.x86=C1FA4
bMultimonAllowed.x86  =C1FA8
ulMaxDebugSessions.x86=C1FAC
bFUSEnabled.x86       =C1FB0
bServerSku.x64        =E63D0
lMaxUserSessions.x64  =E63D4
bAppServerAllowed.x64 =E63D8
bInitialized.x64      =E7470
bRemoteConnAllowed.x64=E7474
bMultimonAllowed.x64  =E7478
ulMaxDebugSessions.x64=E747C
bFUSEnabled.x64       =E7480

[10.0.14393.4704-SLInit]
bInitialized.x64      =E7470
bServerSku.x64        =E63D0
lMaxUserSessions.x64  =E63D4
bAppServerAllowed.x64 =E63D8
bRemoteConnAllowed.x64=E7474
bMultimonAllowed.x64  =E7478
ulMaxDebugSessions.x64=E747C
bFUSEnabled.x64       =E7480

[10.0.14393.4770-SLInit]
bInitialized.x64      =E7470
bServerSku.x64        =E63D0
lMaxUserSessions.x64  =E63D4
bAppServerAllowed.x64 =E63D8
bRemoteConnAllowed.x64=E7474
bMultimonAllowed.x64  =E7478
ulMaxDebugSessions.x64=E747C
bFUSEnabled.x64       =E7480

[10.0.14393.5127-SLInit]
bInitialized.x64      =E7470
bServerSku.x64        =E63D0
lMaxUserSessions.x64  =E63D4
bAppServerAllowed.x64 =E63D8
bRemoteConnAllowed.x64=E7474
bMultimonAllowed.x64  =E7478
ulMaxDebugSessions.x64=E747C
bFUSEnabled.x64       =E7480

[10.0.14901.1000-SLInit]
bInitialized.x86      =C1F6C
bServerSku.x86        =C1F70
lMaxUserSessions.x86  =C1F74
bAppServerAllowed.x86 =C1F78
bRemoteConnAllowed.x86=C1F7C
bMultimonAllowed.x86  =C1F80
ulMaxDebugSessions.x86=C1F84
bFUSEnabled.x86       =C1F88
bServerSku.x64        =E73D0
lMaxUserSessions.x64  =E73D4
bAppServerAllowed.x64 =E73D8
bInitialized.x64      =E8470
bRemoteConnAllowed.x64=E8474
bMultimonAllowed.x64  =E8478
ulMaxDebugSessions.x64=E847C
bFUSEnabled.x64       =E8480

[10.0.14905.1000-SLInit]
bInitialized.x86      =C1F6C
bServerSku.x86        =C1F70
lMaxUserSessions.x86  =C1F74
bAppServerAllowed.x86 =C1F78
bRemoteConnAllowed.x86=C1F7C
bMultimonAllowed.x86  =C1F80
ulMaxDebugSessions.x86=C1F84
bFUSEnabled.x86       =C1F88
bServerSku.x64        =E73D0
lMaxUserSessions.x64  =E73D4
bAppServerAllowed.x64 =E73D8
bInitialized.x64      =E8470
bRemoteConnAllowed.x64=E8474
bMultimonAllowed.x64  =E8478
ulMaxDebugSessions.x64=E847C
bFUSEnabled.x64       =E8480

[10.0.14915.1000-SLInit]
bInitialized.x86      =C4F6C
bServerSku.x86        =C4F70
lMaxUserSessions.x86  =C4F74
bAppServerAllowed.x86 =C4F78
bRemoteConnAllowed.x86=C4F7C
bMultimonAllowed.x86  =C4F80
ulMaxDebugSessions.x86=C4F84
bFUSEnabled.x86       =C4F88
bServerSku.x64        =E93D0
lMaxUserSessions.x64  =E93D4
bAppServerAllowed.x64 =E93D8
bInitialized.x64      =EA470
bRemoteConnAllowed.x64=EA474
bMultimonAllowed.x64  =EA478
ulMaxDebugSessions.x64=EA47C
bFUSEnabled.x64       =EA480

[10.0.14926.1000-SLInit]
bInitialized.x86      =C4F6C
bServerSku.x86        =C4F70
lMaxUserSessions.x86  =C4F74
bAppServerAllowed.x86 =C4F78
bRemoteConnAllowed.x86=C4F7C
bMultimonAllowed.x86  =C4F80
ulMaxDebugSessions.x86=C4F84
bFUSEnabled.x86       =C4F88
bServerSku.x64        =E93D0
lMaxUserSessions.x64  =E93D4
bAppServerAllowed.x64 =E93D8
bInitialized.x64      =EA470
bRemoteConnAllowed.x64=EA474
bMultimonAllowed.x64  =EA478
ulMaxDebugSessions.x64=EA47C
bFUSEnabled.x64       =EA480

[10.0.14931.1000-SLInit]
bInitialized.x86      =C1F6C
bServerSku.x86        =C1F70
lMaxUserSessions.x86  =C1F74
bAppServerAllowed.x86 =C1F78
bRemoteConnAllowed.x86=C1F7C
bMultimonAllowed.x86  =C1F80
ulMaxDebugSessions.x86=C1F84
bFUSEnabled.x86       =C1F88
bServerSku.x64        =E63D0
lMaxUserSessions.x64  =E63D4
bAppServerAllowed.x64 =E63D8
bInitialized.x64      =E7470
bRemoteConnAllowed.x64=E7474
bMultimonAllowed.x64  =E7478
ulMaxDebugSessions.x64=E747C
bFUSEnabled.x64       =E7480

[10.0.14936.1000-SLInit]
bInitialized.x86      =C0F6C
bServerSku.x86        =C0F70
lMaxUserSessions.x86  =C0F74
bAppServerAllowed.x86 =C0F78
bRemoteConnAllowed.x86=C0F7C
bMultimonAllowed.x86  =C0F80
ulMaxDebugSessions.x86=C0F84
bFUSEnabled.x86       =C0F88
bInitialized.x64      =E8460
bRemoteConnAllowed.x64=E8464
bMultimonAllowed.x64  =E8468
ulMaxDebugSessions.x64=E846C
bFUSEnabled.x64       =E8470
bServerSku.x64        =E847C
lMaxUserSessions.x64  =E8480
bAppServerAllowed.x64 =E8484

[10.0.14942.1000-SLInit]
bInitialized.x86      =C0F6C
bServerSku.x86        =C0F70
lMaxUserSessions.x86  =C0F74
bAppServerAllowed.x86 =C0F78
bRemoteConnAllowed.x86=C0F7C
bMultimonAllowed.x86  =C0F80
ulMaxDebugSessions.x86=C0F84
bFUSEnabled.x86       =C0F88
bInitialized.x64      =EC460
bRemoteConnAllowed.x64=EC464
bMultimonAllowed.x64  =EC468
ulMaxDebugSessions.x64=EC46C
bFUSEnabled.x64       =EC470
bServerSku.x64        =EC47C
lMaxUserSessions.x64  =EC480
bAppServerAllowed.x64 =EC484

[10.0.14946.1000-SLInit]
bInitialized.x86      =C0F6C
bServerSku.x86        =C0F70
lMaxUserSessions.x86  =C0F74
bAppServerAllowed.x86 =C0F78
bRemoteConnAllowed.x86=C0F7C
bMultimonAllowed.x86  =C0F80
ulMaxDebugSessions.x86=C0F84
bFUSEnabled.x86       =C0F88
bInitialized.x64      =EC460
bRemoteConnAllowed.x64=EC464
bMultimonAllowed.x64  =EC468
ulMaxDebugSessions.x64=EC46C
bFUSEnabled.x64       =EC470
bServerSku.x64        =EC47C
lMaxUserSessions.x64  =EC480
bAppServerAllowed.x64 =EC484

[10.0.14951.1000-SLInit]
bInitialized.x86      =C5F68
bServerSku.x86        =C5F6C
lMaxUserSessions.x86  =C5F70
bAppServerAllowed.x86 =C5F74
bRemoteConnAllowed.x86=C5F78
bMultimonAllowed.x86  =C5F7C
ulMaxDebugSessions.x86=C5F80
bFUSEnabled.x86       =C5F84
bServerSku.x64        =EF3D0
lMaxUserSessions.x64  =EF3D4
bAppServerAllowed.x64 =EF3D8
bInitialized.x64      =F0470
bRemoteConnAllowed.x64=F0474
bMultimonAllowed.x64  =F0478
ulMaxDebugSessions.x64=F047C
bFUSEnabled.x64       =F0480

[10.0.14955.1000-SLInit]
bInitialized.x86      =C5F68
bServerSku.x86        =C5F6C
lMaxUserSessions.x86  =C5F70
bAppServerAllowed.x86 =C5F74
bRemoteConnAllowed.x86=C5F78
bMultimonAllowed.x86  =C5F7C
ulMaxDebugSessions.x86=C5F80
bFUSEnabled.x86       =C5F84
bServerSku.x64        =EF3D0
lMaxUserSessions.x64  =EF3D4
bAppServerAllowed.x64 =EF3D8
bInitialized.x64      =F0470
bRemoteConnAllowed.x64=F0474
bMultimonAllowed.x64  =F0478
ulMaxDebugSessions.x64=F047C
bFUSEnabled.x64       =F0480

[10.0.14959.1000-SLInit]
bInitialized.x86      =C4F68
bServerSku.x86        =C4F6C
lMaxUserSessions.x86  =C4F70
bAppServerAllowed.x86 =C4F74
bRemoteConnAllowed.x86=C4F78
bMultimonAllowed.x86  =C4F7C
ulMaxDebugSessions.x86=C4F80
bFUSEnabled.x86       =C4F84
bServerSku.x64        =EE3D0
lMaxUserSessions.x64  =EE3D4
bAppServerAllowed.x64 =EE3D8
bInitialized.x64      =EF470
bRemoteConnAllowed.x64=EF474
bMultimonAllowed.x64  =EF478
ulMaxDebugSessions.x64=EF47C
bFUSEnabled.x64       =EF480

[10.0.14965.1001-SLInit]
bInitialized.x86      =C5F68
bServerSku.x86        =C5F6C
lMaxUserSessions.x86  =C5F70
bAppServerAllowed.x86 =C5F74
bRemoteConnAllowed.x86=C5F78
bMultimonAllowed.x86  =C5F7C
ulMaxDebugSessions.x86=C5F80
bFUSEnabled.x86       =C5F84
bInitialized.x64      =EF460
bRemoteConnAllowed.x64=EF464
bMultimonAllowed.x64  =EF468
ulMaxDebugSessions.x64=EF46C
bFUSEnabled.x64       =EF470
bServerSku.x64        =EF47C
lMaxUserSessions.x64  =EF480
bAppServerAllowed.x64 =EF484

[10.0.14971.1000-SLInit]
bInitialized.x86      =C5F68
bServerSku.x86        =C5F6C
lMaxUserSessions.x86  =C5F70
bAppServerAllowed.x86 =C5F74
bRemoteConnAllowed.x86=C5F78
bMultimonAllowed.x86  =C5F7C
ulMaxDebugSessions.x86=C5F80
bFUSEnabled.x86       =C5F84
bServerSku.x64        =EE3C0
lMaxUserSessions.x64  =EE3C4
bAppServerAllowed.x64 =EE3C8
bInitialized.x64      =EE470
bRemoteConnAllowed.x64=EE474
bMultimonAllowed.x64  =EE478
ulMaxDebugSessions.x64=EE47C
bFUSEnabled.x64       =EE480

[10.0.14986.1000-SLInit]
bInitialized.x86      =C5F68
bServerSku.x86        =C5F6C
lMaxUserSessions.x86  =C5F70
bAppServerAllowed.x86 =C5F74
bRemoteConnAllowed.x86=C5F78
bMultimonAllowed.x86  =C5F7C
ulMaxDebugSessions.x86=C5F80
bFUSEnabled.x86       =C5F84
bServerSku.x64        =EE3C0
lMaxUserSessions.x64  =EE3C4
bAppServerAllowed.x64 =EE3C8
bInitialized.x64      =EE470
bRemoteConnAllowed.x64=EE474
bMultimonAllowed.x64  =EE478
ulMaxDebugSessions.x64=EE47C
bFUSEnabled.x64       =EE480

[10.0.14997.1001-SLInit]
bServerSku.x64        =F0408
lMaxUserSessions.x64  =F040C
bAppServerAllowed.x64 =F0410
bInitialized.x64      =F0480
bRemoteConnAllowed.x64=F0484
bMultimonAllowed.x64  =F0488
ulMaxDebugSessions.x64=F048C
bFUSEnabled.x64       =F0490

[10.0.15002.1001-SLInit]
bInitialized.x86      =C6F74
bServerSku.x86        =C6F78
lMaxUserSessions.x86  =C6F7C
bAppServerAllowed.x86 =C6F80
bRemoteConnAllowed.x86=C6F84
bMultimonAllowed.x86  =C6F88
ulMaxDebugSessions.x86=C6F8C
bFUSEnabled.x86       =C6F90
bServerSku.x64        =F0408
lMaxUserSessions.x64  =F040C
bAppServerAllowed.x64 =F0410
bInitialized.x64      =F0480
bRemoteConnAllowed.x64=F0484
bMultimonAllowed.x64  =F0488
ulMaxDebugSessions.x64=F048C
bFUSEnabled.x64       =F0490

[10.0.15007.1000-SLInit]
bInitialized.x86      =C6F74
bServerSku.x86        =C6F78
lMaxUserSessions.x86  =C6F7C
bAppServerAllowed.x86 =C6F80
bRemoteConnAllowed.x86=C6F84
bMultimonAllowed.x86  =C6F88
ulMaxDebugSessions.x86=C6F8C
bFUSEnabled.x86       =C6F90
bServerSku.x64        =F0408
lMaxUserSessions.x64  =F040C
bAppServerAllowed.x64 =F0410
bInitialized.x64      =F0480
bRemoteConnAllowed.x64=F0484
bMultimonAllowed.x64  =F0488
ulMaxDebugSessions.x64=F048C
bFUSEnabled.x64       =F0490

[10.0.15014.1000-SLInit]
bInitialized.x86      =C6F74
bServerSku.x86        =C6F78
lMaxUserSessions.x86  =C6F7C
bAppServerAllowed.x86 =C6F80
bRemoteConnAllowed.x86=C6F84
bMultimonAllowed.x86  =C6F88
ulMaxDebugSessions.x86=C6F8C
bFUSEnabled.x86       =C6F90
bServerSku.x64        =F0408
lMaxUserSessions.x64  =F040C
bAppServerAllowed.x64 =F0410
bInitialized.x64      =F0480
bRemoteConnAllowed.x64=F0484
bMultimonAllowed.x64  =F0488
ulMaxDebugSessions.x64=F048C
bFUSEnabled.x64       =F0490

[10.0.15019.1000-SLInit]
bInitialized.x86      =C5F68
bServerSku.x86        =C5F6C
lMaxUserSessions.x86  =C5F70
bAppServerAllowed.x86 =C5F74
bRemoteConnAllowed.x86=C5F78
bMultimonAllowed.x86  =C5F7C
ulMaxDebugSessions.x86=C5F80
bFUSEnabled.x86       =C5F84
bServerSku.x64        =ECBDC
lMaxUserSessions.x64  =ECBE0
bAppServerAllowed.x64 =ECBE4
bInitialized.x64      =F0490
bRemoteConnAllowed.x64=F0494
bMultimonAllowed.x64  =F0498
ulMaxDebugSessions.x64=F049C
bFUSEnabled.x64       =F04A0

[10.0.15025.1000-SLInit]
bServerSku.x64        =EE3E0
lMaxUserSessions.x64  =EE3E4
bAppServerAllowed.x64 =EE3E8
bInitialized.x64      =EF488
bRemoteConnAllowed.x64=EF48C
bMultimonAllowed.x64  =EF490
ulMaxDebugSessions.x64=EF494
bFUSEnabled.x64       =EF498

[10.0.15031.0-SLInit]
bInitialized.x86      =C2F6C
bServerSku.x86        =C2F70
lMaxUserSessions.x86  =C2F74
bAppServerAllowed.x86 =C2F78
bRemoteConnAllowed.x86=C2F7C
bMultimonAllowed.x86  =C2F80
ulMaxDebugSessions.x86=C2F84
bFUSEnabled.x86       =C2F88
bServerSku.x64        =E93E0
lMaxUserSessions.x64  =E93E4
bAppServerAllowed.x64 =E93E8
bInitialized.x64      =EA488
bRemoteConnAllowed.x64=EA48C
bMultimonAllowed.x64  =EA490
ulMaxDebugSessions.x64=EA494
bFUSEnabled.x64       =EA498

[10.0.15042.0-SLInit]
bInitialized.x86      =C2F6C
bServerSku.x86        =C2F70
lMaxUserSessions.x86  =C2F74
bAppServerAllowed.x86 =C2F78
bRemoteConnAllowed.x86=C2F7C
bMultimonAllowed.x86  =C2F80
ulMaxDebugSessions.x86=C2F84
bFUSEnabled.x86       =C2F88
bServerSku.x64        =E93E0
lMaxUserSessions.x64  =E93E4
bAppServerAllowed.x64 =E93E8
bInitialized.x64      =EA488
bRemoteConnAllowed.x64=EA48C
bMultimonAllowed.x64  =EA490
ulMaxDebugSessions.x64=EA494
bFUSEnabled.x64       =EA498

[10.0.15046.0-SLInit]
bInitialized.x86      =C4F18
bServerSku.x86        =C4F1C
lMaxUserSessions.x86  =C4F20
bAppServerAllowed.x86 =C4F24
bRemoteConnAllowed.x86=C4F28
ulMaxDebugSessions.x86=C4F2C
bMultimonAllowed.x86  =C5010
bFUSEnabled.x86       =C5014
bInitialized.x64      =EB468
bRemoteConnAllowed.x64=EB46C
bMultimonAllowed.x64  =EB470
ulMaxDebugSessions.x64=EB474
bFUSEnabled.x64       =EB478
bServerSku.x64        =EB484
lMaxUserSessions.x64  =EB488
bAppServerAllowed.x64 =EB48C

[10.0.15048.0-SLInit]
bInitialized.x86      =C4F18
bServerSku.x86        =C4F1C
lMaxUserSessions.x86  =C4F20
bAppServerAllowed.x86 =C4F24
bRemoteConnAllowed.x86=C4F28
ulMaxDebugSessions.x86=C4F2C
bMultimonAllowed.x86  =C5010
bFUSEnabled.x86       =C5014
bInitialized.x64      =EB468
bRemoteConnAllowed.x64=EB46C
bMultimonAllowed.x64  =EB470
ulMaxDebugSessions.x64=EB474
bFUSEnabled.x64       =EB478
bServerSku.x64        =EB484
lMaxUserSessions.x64  =EB488
bAppServerAllowed.x64 =EB48C

[10.0.15055.0-SLInit]
bInitialized.x86      =C2F70
bServerSku.x86        =C2F74
lMaxUserSessions.x86  =C2F78
bAppServerAllowed.x86 =C2F7C
bRemoteConnAllowed.x86=C2F80
bMultimonAllowed.x86  =C2F84
ulMaxDebugSessions.x86=C2F88
bFUSEnabled.x86       =C2F8C
bServerSku.x64        =E83D8
lMaxUserSessions.x64  =E83DC
bAppServerAllowed.x64 =E83E0
bInitialized.x64      =E9490
bRemoteConnAllowed.x64=E9494
bMultimonAllowed.x64  =E9498
ulMaxDebugSessions.x64=E949C
bFUSEnabled.x64       =E94A0

[10.0.15058.0-SLInit]
bInitialized.x86      =C2F70
bServerSku.x86        =C2F74
lMaxUserSessions.x86  =C2F78
bAppServerAllowed.x86 =C2F7C
bRemoteConnAllowed.x86=C2F80
bMultimonAllowed.x86  =C2F84
ulMaxDebugSessions.x86=C2F88
bFUSEnabled.x86       =C2F8C
bInitialized.x64      =E9468
bRemoteConnAllowed.x64=E946C
bMultimonAllowed.x64  =E9470
ulMaxDebugSessions.x64=E9474
bFUSEnabled.x64       =E9478
bServerSku.x64        =E9484
lMaxUserSessions.x64  =E9488
bAppServerAllowed.x64 =E948C

[10.0.15061.0-SLInit]
bInitialized.x86      =C2F70
bServerSku.x86        =C2F74
lMaxUserSessions.x86  =C2F78
bAppServerAllowed.x86 =C2F7C
bRemoteConnAllowed.x86=C2F80
bMultimonAllowed.x86  =C2F84
ulMaxDebugSessions.x86=C2F88
bFUSEnabled.x86       =C2F8C
bInitialized.x64      =E9468
bRemoteConnAllowed.x64=E946C
bMultimonAllowed.x64  =E9470
ulMaxDebugSessions.x64=E9474
bFUSEnabled.x64       =E9478
bServerSku.x64        =E9484
lMaxUserSessions.x64  =E9488
bAppServerAllowed.x64 =E948C

[10.0.15063.0-SLInit]
bInitialized.x86      =C2F70
bServerSku.x86        =C2F74
lMaxUserSessions.x86  =C2F78
bAppServerAllowed.x86 =C2F7C
bRemoteConnAllowed.x86=C2F80
bMultimonAllowed.x86  =C2F84
ulMaxDebugSessions.x86=C2F88
bFUSEnabled.x86       =C2F8C
bInitialized.x64      =E9468
bRemoteConnAllowed.x64=E946C
bMultimonAllowed.x64  =E9470
ulMaxDebugSessions.x64=E9474
bFUSEnabled.x64       =E9478
bServerSku.x64        =E9484
lMaxUserSessions.x64  =E9488
bAppServerAllowed.x64 =E948C

[10.0.15063.296-SLInit]
bInitialized.x86      =C2F70
bServerSku.x86        =C2F74
lMaxUserSessions.x86  =C2F78
bAppServerAllowed.x86 =C2F7C
bRemoteConnAllowed.x86=C2F80
bMultimonAllowed.x86  =C2F84
ulMaxDebugSessions.x86=C2F88
bFUSEnabled.x86       =C2F8C
bInitialized.x64      =E9468
bRemoteConnAllowed.x64=E946C
bMultimonAllowed.x64  =E9470
ulMaxDebugSessions.x64=E9474
bFUSEnabled.x64       =E9478
bServerSku.x64        =E9484
lMaxUserSessions.x64  =E9488
bAppServerAllowed.x64 =E948C

[10.0.15063.994-SLInit]
bInitialized.x64      =E9468
bRemoteConnAllowed.x64=E946C
bMultimonAllowed.x64  =E9470
ulMaxDebugSessions.x64=E9474
bFUSEnabled.x64       =E9478
bServerSku.x64        =E9484
lMaxUserSessions.x64  =E9488
bAppServerAllowed.x64 =E948C

[10.0.15063.1155-SLInit]
bInitialized.x64      =E9468
bRemoteConnAllowed.x64=E946C
bMultimonAllowed.x64  =E9470
ulMaxDebugSessions.x64=E9474
bFUSEnabled.x64       =E9478
bServerSku.x64        =E9484
lMaxUserSessions.x64  =E9488
bAppServerAllowed.x64 =E948C

[10.0.15063.1746-SLInit]
bInitialized.x86      =C3F98
bServerSku.x86        =C3F9C
lMaxUserSessions.x86  =C3FA0
bAppServerAllowed.x86 =C3FA4
bRemoteConnAllowed.x86=C3FA8
bMultimonAllowed.x86  =C3FAC
ulMaxDebugSessions.x86=C3FB0
bFUSEnabled.x86       =C3FB4
bInitialized.x64      =E9468
bRemoteConnAllowed.x64=E946C
bMultimonAllowed.x64  =E9470
ulMaxDebugSessions.x64=E9474
bFUSEnabled.x64       =E9478
bServerSku.x64        =E9484
lMaxUserSessions.x64  =E9488
bAppServerAllowed.x64 =E948C

[10.0.15063.2283-SLInit]
; no x86-version
bInitialized.x64      =E9468
bRemoteConnAllowed.x64=E946C
bMultimonAllowed.x64  =E9470
ulMaxDebugSessions.x64=E9474
bFUSEnabled.x64       =E9478
bServerSku.x64        =E9484
lMaxUserSessions.x64  =E9488
bAppServerAllowed.x64 =E948C

[10.0.16179.1000-SLInit]
bInitialized.x86      =C7F6C
bServerSku.x86        =C7F70
lMaxUserSessions.x86  =C7F74
bAppServerAllowed.x86 =C7F78
bRemoteConnAllowed.x86=C7F7C
bMultimonAllowed.x86  =C7F80
ulMaxDebugSessions.x86=C7F84
bFUSEnabled.x86       =C7F88
bServerSku.x64        =E83D8
lMaxUserSessions.x64  =E83DC
bAppServerAllowed.x64 =E83E0
bInitialized.x64      =E9490
bRemoteConnAllowed.x64=E9494
bMultimonAllowed.x64  =E9498
ulMaxDebugSessions.x64=E949C
bFUSEnabled.x64       =E94A0

[10.0.16184.1001-SLInit]
bInitialized.x86      =C7F6C
bServerSku.x86        =C7F70
lMaxUserSessions.x86  =C7F74
bAppServerAllowed.x86 =C7F78
bRemoteConnAllowed.x86=C7F7C
bMultimonAllowed.x86  =C7F80
ulMaxDebugSessions.x86=C7F84
bFUSEnabled.x86       =C7F88
bServerSku.x64        =E83D8
lMaxUserSessions.x64  =E83DC
bAppServerAllowed.x64 =E83E0
bInitialized.x64      =E9490
bRemoteConnAllowed.x64=E9494
bMultimonAllowed.x64  =E9498
ulMaxDebugSessions.x64=E949C
bFUSEnabled.x64       =E94A0

[10.0.16199.1000-SLInit]
bInitialized.x86      =C8F74
bServerSku.x86        =C8F78
lMaxUserSessions.x86  =C8F7C
bAppServerAllowed.x86 =C8F80
bRemoteConnAllowed.x86=C8F84
bMultimonAllowed.x86  =C8F88
ulMaxDebugSessions.x86=C8F8C
bFUSEnabled.x86       =C8F90
bServerSku.x64        =E83E8
lMaxUserSessions.x64  =E83EC
bAppServerAllowed.x64 =E83F0
bInitialized.x64      =E94A0
bRemoteConnAllowed.x64=E94A4
bMultimonAllowed.x64  =E94A8
ulMaxDebugSessions.x64=E94AC
bFUSEnabled.x64       =E94B0

[10.0.16215.1000-SLInit]
bInitialized.x86      =C5F78
bServerSku.x86        =C5F7C
lMaxUserSessions.x86  =C5F80
bAppServerAllowed.x86 =C5F84
bRemoteConnAllowed.x86=C5F88
bMultimonAllowed.x86  =C5F8C
ulMaxDebugSessions.x86=C5F90
bFUSEnabled.x86       =C5F94
bServerSku.x64        =EA3E8
lMaxUserSessions.x64  =EA3EC
bAppServerAllowed.x64 =EA3F0
bInitialized.x64      =EB4A0
bRemoteConnAllowed.x64=EB4A4
bMultimonAllowed.x64  =EB4A8
ulMaxDebugSessions.x64=EB4AC
bFUSEnabled.x64       =EB4B0

[10.0.16232.1000-SLInit]
bInitialized.x86      =C5F78
bServerSku.x86        =C5F7C
lMaxUserSessions.x86  =C5F80
bAppServerAllowed.x86 =C5F84
bRemoteConnAllowed.x86=C5F88
bMultimonAllowed.x86  =C5F8C
ulMaxDebugSessions.x86=C5F90
bFUSEnabled.x86       =C5F94
bServerSku.x64        =EA3E8
lMaxUserSessions.x64  =EA3EC
bAppServerAllowed.x64 =EA3F0
bInitialized.x64      =EB4A0
bRemoteConnAllowed.x64=EB4A4
bMultimonAllowed.x64  =EB4A8
ulMaxDebugSessions.x64=EB4AC
bFUSEnabled.x64       =EB4B0

[10.0.16237.1001-SLInit]
bInitialized.x86      =C5F78
bServerSku.x86        =C5F7C
lMaxUserSessions.x86  =C5F80
bAppServerAllowed.x86 =C5F84
bRemoteConnAllowed.x86=C5F88
bMultimonAllowed.x86  =C5F8C
ulMaxDebugSessions.x86=C5F90
bFUSEnabled.x86       =C5F94
bServerSku.x64        =EB3EC
lMaxUserSessions.x64  =EB3F0
bAppServerAllowed.x64 =EB3F4
bInitialized.x64      =EC4A0
bRemoteConnAllowed.x64=EC4A4
bMultimonAllowed.x64  =EC4A8
ulMaxDebugSessions.x64=EC4AC
bFUSEnabled.x64       =EC4B0

[10.0.16241.1001-SLInit]
bInitialized.x86      =C5F78
bServerSku.x86        =C5F7C
lMaxUserSessions.x86  =C5F80
bAppServerAllowed.x86 =C5F84
bRemoteConnAllowed.x86=C5F88
bMultimonAllowed.x86  =C5F8C
ulMaxDebugSessions.x86=C5F90
bFUSEnabled.x86       =C5F94
bServerSku.x64        =EB3EC
lMaxUserSessions.x64  =EB3F0
bAppServerAllowed.x64 =EB3F4
bInitialized.x64      =EC4A0
bRemoteConnAllowed.x64=EC4A4
bMultimonAllowed.x64  =EC4A8
ulMaxDebugSessions.x64=EC4AC
bFUSEnabled.x64       =EC4B0

[10.0.16251.0-SLInit]
bInitialized.x86      =C9F78
bServerSku.x86        =C9F7C
lMaxUserSessions.x86  =C9F80
bAppServerAllowed.x86 =C9F84
bRemoteConnAllowed.x86=C9F88
bMultimonAllowed.x86  =C9F8C
ulMaxDebugSessions.x86=C9F90
bFUSEnabled.x86       =C9F94
bServerSku.x64        =EB3EC
lMaxUserSessions.x64  =EB3F0
bAppServerAllowed.x64 =EB3F4
bInitialized.x64      =EC4A0
bRemoteConnAllowed.x64=EC4A4
bMultimonAllowed.x64  =EC4A8
ulMaxDebugSessions.x64=EC4AC
bFUSEnabled.x64       =EC4B0

[10.0.16251.1000-SLInit]
bInitialized.x86      =C9F78
bServerSku.x86        =C9F7C
lMaxUserSessions.x86  =C9F80
bAppServerAllowed.x86 =C9F84
bRemoteConnAllowed.x86=C9F88
bMultimonAllowed.x86  =C9F8C
ulMaxDebugSessions.x86=C9F90
bFUSEnabled.x86       =C9F94
bServerSku.x64        =EB3EC
lMaxUserSessions.x64  =EB3F0
bAppServerAllowed.x64 =EB3F4
bInitialized.x64      =EC4A0
bRemoteConnAllowed.x64=EC4A4
bMultimonAllowed.x64  =EC4A8
ulMaxDebugSessions.x64=EC4AC
bFUSEnabled.x64       =EC4B0

[10.0.16257.1-SLInit]
bInitialized.x86      =C9F7C
bServerSku.x86        =C9F80
lMaxUserSessions.x86  =C9F84
bAppServerAllowed.x86 =C9F88
bRemoteConnAllowed.x86=C9F8C
bMultimonAllowed.x86  =C9F90
ulMaxDebugSessions.x86=C9F94
bFUSEnabled.x86       =C9F98
bServerSku.x64        =EB3F0
lMaxUserSessions.x64  =EB3F4
bAppServerAllowed.x64 =EB3F8
bInitialized.x64      =EC4A0
bRemoteConnAllowed.x64=EC4A4
bMultimonAllowed.x64  =EC4A8
ulMaxDebugSessions.x64=EC4AC
bFUSEnabled.x64       =EC4B0

[10.0.16257.1000-SLInit]
bInitialized.x86      =C9F7C
bServerSku.x86        =C9F80
lMaxUserSessions.x86  =C9F84
bAppServerAllowed.x86 =C9F88
bRemoteConnAllowed.x86=C9F8C
bMultimonAllowed.x86  =C9F90
ulMaxDebugSessions.x86=C9F94
bFUSEnabled.x86       =C9F98
bServerSku.x64        =EB3F0
lMaxUserSessions.x64  =EB3F4
bAppServerAllowed.x64 =EB3F8
bInitialized.x64      =EC4A0
bRemoteConnAllowed.x64=EC4A4
bMultimonAllowed.x64  =EC4A8
ulMaxDebugSessions.x64=EC4AC
bFUSEnabled.x64       =EC4B0

[10.0.16273.1000-SLInit]
bInitialized.x86      =C9F7C
bServerSku.x86        =C9F80
lMaxUserSessions.x86  =C9F84
bAppServerAllowed.x86 =C9F88
bRemoteConnAllowed.x86=C9F8C
bMultimonAllowed.x86  =C9F90
ulMaxDebugSessions.x86=C9F94
bFUSEnabled.x86       =C9F98
bServerSku.x64        =EB3F0
lMaxUserSessions.x64  =EB3F4
bAppServerAllowed.x64 =EB3F8
bInitialized.x64      =EC4A0
bRemoteConnAllowed.x64=EC4A4
bMultimonAllowed.x64  =EC4A8
ulMaxDebugSessions.x64=EC4AC
bFUSEnabled.x64       =EC4B0

[10.0.16275.1000-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.16278.1000-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.16281.1000-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.16288.1-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.16291.0-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.16294.1-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.16296.0-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.16299.0-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.16299.15-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.16299.1087-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.16353.1000-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.16362.1000-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.17004.1000-SLInit]
bInitialized.x86      =C6F7C
bServerSku.x86        =C6F80
lMaxUserSessions.x86  =C6F84
bAppServerAllowed.x86 =C6F88
bRemoteConnAllowed.x86=C6F8C
bMultimonAllowed.x86  =C6F90
ulMaxDebugSessions.x86=C6F94
bFUSEnabled.x86       =C6F98
bServerSku.x64        =ED3E8
lMaxUserSessions.x64  =ED3EC
bAppServerAllowed.x64 =ED3F0
bInitialized.x64      =EE4A0
bRemoteConnAllowed.x64=EE4A4
bMultimonAllowed.x64  =EE4A8
ulMaxDebugSessions.x64=EE4AC
bFUSEnabled.x64       =EE4B0

[10.0.17017.1000-SLInit]
bInitialized.x86      =C9EB8
bServerSku.x86        =C9EBC
lMaxUserSessions.x86  =C9EC0
bAppServerAllowed.x86 =C9EC4
bRemoteConnAllowed.x86=C9EC8
bMultimonAllowed.x86  =C9ECC
ulMaxDebugSessions.x86=C9ED0
bFUSEnabled.x86       =C9ED4
bServerSku.x64        =EC2E8
lMaxUserSessions.x64  =EC2EC
bAppServerAllowed.x64 =EC2F0
bInitialized.x64      =ED3A0
bRemoteConnAllowed.x64=ED3A4
bMultimonAllowed.x64  =ED3A8
ulMaxDebugSessions.x64=ED3AC
bFUSEnabled.x64       =ED3B0

[10.0.17025.1000-SLInit]
bInitialized.x86      =C9EB8
bServerSku.x86        =C9EBC
lMaxUserSessions.x86  =C9EC0
bAppServerAllowed.x86 =C9EC4
bRemoteConnAllowed.x86=C9EC8
bMultimonAllowed.x86  =C9ECC
ulMaxDebugSessions.x86=C9ED0
bFUSEnabled.x86       =C9ED4
bServerSku.x64        =EC2E8
lMaxUserSessions.x64  =EC2EC
bAppServerAllowed.x64 =EC2F0
bInitialized.x64      =ED3A0
bRemoteConnAllowed.x64=ED3A4
bMultimonAllowed.x64  =ED3A8
ulMaxDebugSessions.x64=ED3AC
bFUSEnabled.x64       =ED3B0

[10.0.17035.1000-SLInit]
bInitialized.x86      =C9ED8
bServerSku.x86        =C9EDC
lMaxUserSessions.x86  =C9EE0
bAppServerAllowed.x86 =C9EE4
bRemoteConnAllowed.x86=C9EE8
bMultimonAllowed.x86  =C9EEC
ulMaxDebugSessions.x86=C9EF0
bFUSEnabled.x86       =C9EF4
bServerSku.x64        =EC2E8
lMaxUserSessions.x64  =EC2EC
bAppServerAllowed.x64 =EC2F0
bInitialized.x64      =ED3A0
bRemoteConnAllowed.x64=ED3A4
bMultimonAllowed.x64  =ED3A8
ulMaxDebugSessions.x64=ED3AC
bFUSEnabled.x64       =ED3B0

[10.0.17046.1000-SLInit]
bInitialized.x86      =C9ED8
bServerSku.x86        =C9EDC
lMaxUserSessions.x86  =C9EE0
bAppServerAllowed.x86 =C9EE4
bRemoteConnAllowed.x86=C9EE8
bMultimonAllowed.x86  =C9EEC
ulMaxDebugSessions.x86=C9EF0
bFUSEnabled.x86       =C9EF4
bServerSku.x64        =EC2E8
lMaxUserSessions.x64  =EC2EC
bAppServerAllowed.x64 =EC2F0
bInitialized.x64      =ED3A0
bRemoteConnAllowed.x64=ED3A4
bMultimonAllowed.x64  =ED3A8
ulMaxDebugSessions.x64=ED3AC
bFUSEnabled.x64       =ED3B0

[10.0.17063.1000-SLInit]
bInitialized.x86      =CBF38
bServerSku.x86        =CBF3C
lMaxUserSessions.x86  =CBF40
bAppServerAllowed.x86 =CBF44
bRemoteConnAllowed.x86=CBF48
bMultimonAllowed.x86  =CBF4C
ulMaxDebugSessions.x86=CBF50
bFUSEnabled.x86       =CBF54
bServerSku.x64        =F1378
lMaxUserSessions.x64  =F137C
bAppServerAllowed.x64 =F1380
bInitialized.x64      =F2430
bRemoteConnAllowed.x64=F2434
bMultimonAllowed.x64  =F2438
ulMaxDebugSessions.x64=F243C
bFUSEnabled.x64       =F2440

[10.0.17115.1-SLInit]
bInitialized.x86      =CBF38
bServerSku.x86        =CBF3C
lMaxUserSessions.x86  =CBF40
bAppServerAllowed.x86 =CBF44
bRemoteConnAllowed.x86=CBF48
bMultimonAllowed.x86  =CBF4C
ulMaxDebugSessions.x86=CBF50
bFUSEnabled.x86       =CBF54
bServerSku.x64        =F1378
lMaxUserSessions.x64  =F137C
bAppServerAllowed.x64 =F1380
bInitialized.x64      =F2430
bRemoteConnAllowed.x64=F2434
bMultimonAllowed.x64  =F2438
ulMaxDebugSessions.x64=F243C
bFUSEnabled.x64       =F2440

[10.0.17128.1-SLInit]
bInitialized.x86      =CBF38
bServerSku.x86        =CBF3C
lMaxUserSessions.x86  =CBF40
bAppServerAllowed.x86 =CBF44
bRemoteConnAllowed.x86=CBF48
bMultimonAllowed.x86  =CBF4C
ulMaxDebugSessions.x86=CBF50
bFUSEnabled.x86       =CBF54
bServerSku.x64        =F1378
lMaxUserSessions.x64  =F137C
bAppServerAllowed.x64 =F1380
bInitialized.x64      =F2430
bRemoteConnAllowed.x64=F2434
bMultimonAllowed.x64  =F2438
ulMaxDebugSessions.x64=F243C
bFUSEnabled.x64       =F2440

[10.0.17133.1-SLInit]
bInitialized.x86      =CBF38
bServerSku.x86        =CBF3C
lMaxUserSessions.x86  =CBF40
bAppServerAllowed.x86 =CBF44
bRemoteConnAllowed.x86=CBF48
bMultimonAllowed.x86  =CBF4C
ulMaxDebugSessions.x86=CBF50
bFUSEnabled.x86       =CBF54
bServerSku.x64        =F1378
lMaxUserSessions.x64  =F137C
bAppServerAllowed.x64 =F1380
bInitialized.x64      =F2430
bRemoteConnAllowed.x64=F2434
bMultimonAllowed.x64  =F2438
ulMaxDebugSessions.x64=F243C
bFUSEnabled.x64       =F2440

[10.0.17134.1-SLInit]
bInitialized.x86      =CBF38
bServerSku.x86        =CBF3C
lMaxUserSessions.x86  =CBF40
bAppServerAllowed.x86 =CBF44
bRemoteConnAllowed.x86=CBF48
bMultimonAllowed.x86  =CBF4C
ulMaxDebugSessions.x86=CBF50
bFUSEnabled.x86       =CBF54
bServerSku.x64        =F1378
lMaxUserSessions.x64  =F137C
bAppServerAllowed.x64 =F1380
bInitialized.x64      =F2430
bRemoteConnAllowed.x64=F2434
bMultimonAllowed.x64  =F2438
ulMaxDebugSessions.x64=F243C
bFUSEnabled.x64       =F2440

[10.0.17134.706-SLInit]
bInitialized.x86      =CBF38
bServerSku.x86        =CBF3C
lMaxUserSessions.x86  =CBF40
bAppServerAllowed.x86 =CBF44
bRemoteConnAllowed.x86=CBF48
bMultimonAllowed.x86  =CBF4C
ulMaxDebugSessions.x86=CBF50
bFUSEnabled.x86       =CBF54
bServerSku.x64        =F1378
lMaxUserSessions.x64  =F137C
bAppServerAllowed.x64 =F1380
bInitialized.x64      =F2430
bRemoteConnAllowed.x64=F2434
bMultimonAllowed.x64  =F2438
ulMaxDebugSessions.x64=F243C
bFUSEnabled.x64       =F2440

[10.0.17134.1304-SLInit]
bInitialized.x86      =CBF38
bServerSku.x86        =CBF3C
lMaxUserSessions.x86  =CBF40
bAppServerAllowed.x86 =CBF44
bRemoteConnAllowed.x86=CBF48
bMultimonAllowed.x86  =CBF4C
ulMaxDebugSessions.x86=CBF50
bFUSEnabled.x86       =CBF54
bServerSku.x64        =F1378
lMaxUserSessions.x64  =F137C
bAppServerAllowed.x64 =F1380
bInitialized.x64      =F2430
bRemoteConnAllowed.x64=F2434
bMultimonAllowed.x64  =F2438
ulMaxDebugSessions.x64=F243C
bFUSEnabled.x64       =F2440

[10.0.17134.1967-SLInit]
bServerSku.x64        =F0378
lMaxUserSessions.x64  =F037C
bAppServerAllowed.x64 =F0380
bInitialized.x64      =F1430
bRemoteConnAllowed.x64=F1434
bMultimonAllowed.x64  =F1438
ulMaxDebugSessions.x64=F143C
bFUSEnabled.x64       =F1440

[10.0.17723.1000-SLInit]
bInitialized.x64      =E9AB0
bServerSku.x64        =E9AB4
lMaxUserSessions.x64  =E9AB8
bAppServerAllowed.x64 =E9AC0
bRemoteConnAllowed.x64=E9AC4
bMultimonAllowed.x64  =E9AC8
ulMaxDebugSessions.x64=E9ACC
bFUSEnabled.x64       =E9AD0

[10.0.17738.1000-SLInit]
bInitialized.x64      =EBAB0
bServerSku.x64        =EBAB4
lMaxUserSessions.x64  =EBAB8
bAppServerAllowed.x64 =EBAC0
bRemoteConnAllowed.x64=EBAC4
bMultimonAllowed.x64  =EBAC8
ulMaxDebugSessions.x64=EBACC
bFUSEnabled.x64       =EBAD0

[10.0.17746.1000-SLInit]
bInitialized.x64      =ECAB0
bServerSku.x64        =ECAB4
lMaxUserSessions.x64  =ECAB8
bAppServerAllowed.x64 =ECAC0
bRemoteConnAllowed.x64=ECAC4
bMultimonAllowed.x64  =ECAC8
ulMaxDebugSessions.x64=ECACC
bFUSEnabled.x64       =ECAD0

[10.0.17763.1-SLInit]
bInitialized.x86      =CD798
bServerSku.x86        =CD79C
lMaxUserSessions.x86  =CD7A0
bAppServerAllowed.x86 =CD7A8
bRemoteConnAllowed.x86=CD7AC
bMultimonAllowed.x86  =CD7B0
ulMaxDebugSessions.x86=CD7B4
bFUSEnabled.x86       =CD7B8
bInitialized.x64      =ECAB0
bServerSku.x64        =ECAB4
lMaxUserSessions.x64  =ECAB8
bAppServerAllowed.x64 =ECAC0
bRemoteConnAllowed.x64=ECAC4
bMultimonAllowed.x64  =ECAC8
ulMaxDebugSessions.x64=ECACC
bFUSEnabled.x64       =ECAD0

[10.0.17763.165-SLInit]
bInitialized.x64      =ECAB0
bServerSku.x64        =ECAB4
lMaxUserSessions.x64  =ECAB8
bAppServerAllowed.x64 =ECAC0
bRemoteConnAllowed.x64=ECAC4
bMultimonAllowed.x64  =ECAC8
ulMaxDebugSessions.x64=ECACC
bFUSEnabled.x64       =ECAD0

[10.0.17763.168-SLInit]
bInitialized.x86      =CD798
bServerSku.x86        =CD79C
lMaxUserSessions.x86  =CD7A0
bAppServerAllowed.x86 =CD7A8
bRemoteConnAllowed.x86=CD7AC
bMultimonAllowed.x86  =CD7B0
ulMaxDebugSessions.x86=CD7B4
bFUSEnabled.x86       =CD7B8
bInitialized.x64      =ECAB0
bServerSku.x64        =ECAB4
lMaxUserSessions.x64  =ECAB8
bAppServerAllowed.x64 =ECAC0
bRemoteConnAllowed.x64=ECAC4
bMultimonAllowed.x64  =ECAC8
ulMaxDebugSessions.x64=ECACC
bFUSEnabled.x64       =ECAD0

[10.0.17763.288-SLInit]
bInitialized.x86      =CD798
bServerSku.x86        =CD79C
lMaxUserSessions.x86  =CD7A0
bAppServerAllowed.x86 =CD7A8
bRemoteConnAllowed.x86=CD7AC
bMultimonAllowed.x86  =CD7B0
ulMaxDebugSessions.x86=CD7B4
bFUSEnabled.x86       =CD7B8
bInitialized.x64      =ECAB0
bServerSku.x64        =ECAB4
lMaxUserSessions.x64  =ECAB8
bAppServerAllowed.x64 =ECAC0
bRemoteConnAllowed.x64=ECAC4
bMultimonAllowed.x64  =ECAC8
ulMaxDebugSessions.x64=ECACC
bFUSEnabled.x64       =ECAD0

[10.0.17763.292-SLInit]
bInitialized.x86      =CD798
bServerSku.x86        =CD79C
lMaxUserSessions.x86  =CD7A0
bAppServerAllowed.x86 =CD7A8
bRemoteConnAllowed.x86=CD7AC
bMultimonAllowed.x86  =CD7B0
ulMaxDebugSessions.x86=CD7B4
bFUSEnabled.x86       =CD7B8
bInitialized.x64      =ECAB0
bServerSku.x64        =ECAB4
lMaxUserSessions.x64  =ECAB8
bAppServerAllowed.x64 =ECAC0
bRemoteConnAllowed.x64=ECAC4
bMultimonAllowed.x64  =ECAC8
ulMaxDebugSessions.x64=ECACC
bFUSEnabled.x64       =ECAD0

[10.0.17763.379-SLInit]
bInitialized.x86      =CD798
bServerSku.x86        =CD79C
lMaxUserSessions.x86  =CD7A0
bAppServerAllowed.x86 =CD7A8
bRemoteConnAllowed.x86=CD7AC
bMultimonAllowed.x86  =CD7B0
ulMaxDebugSessions.x86=CD7B4
bFUSEnabled.x86       =CD7B8
bInitialized.x64      =ECAB0
bServerSku.x64        =ECAB4
lMaxUserSessions.x64  =ECAB8
bAppServerAllowed.x64 =ECAC0
bRemoteConnAllowed.x64=ECAC4
bMultimonAllowed.x64  =ECAC8
ulMaxDebugSessions.x64=ECACC
bFUSEnabled.x64       =ECAD0

[10.0.17763.437-SLInit]
bInitialized.x86      =CD798
bServerSku.x86        =CD79C
lMaxUserSessions.x86  =CD7A0
bAppServerAllowed.x86 =CD7A8
bRemoteConnAllowed.x86=CD7AC
bMultimonAllowed.x86  =CD7B0
ulMaxDebugSessions.x86=CD7B4
bFUSEnabled.x86       =CD7B8
bInitialized.x64      =ECAB0
bServerSku.x64        =ECAB4
lMaxUserSessions.x64  =ECAB8
bAppServerAllowed.x64 =ECAC0
bRemoteConnAllowed.x64=ECAC4
bMultimonAllowed.x64  =ECAC8
ulMaxDebugSessions.x64=ECACC
bFUSEnabled.x64       =ECAD0

[10.0.17763.771-SLInit]
bInitialized.x86      =CD79C
bServerSku.x86        =CD7A0
lMaxUserSessions.x86  =CD7A4
bAppServerAllowed.x86 =CD7AC
bRemoteConnAllowed.x86=CD7B0
bMultimonAllowed.x86  =CD7B4
ulMaxDebugSessions.x86=CD7B8
bFUSEnabled.x86       =CD7BC
bServerSku.x64        =ECAB8
lMaxUserSessions.x64  =ECABC
bAppServerAllowed.x64 =ECAC4
bInitialized.x64      =ECAB4
bRemoteConnAllowed.x64=ECAC8
bMultimonAllowed.x64  =ECACC
ulMaxDebugSessions.x64=ECAD0
bFUSEnabled.x64       =ECAD4

[10.0.17763.1369-SLInit]
bInitialized.x86      =CD79C
bServerSku.x86        =CD7A0
lMaxUserSessions.x86  =CD7A4
bAppServerAllowed.x86 =CD7AC
bRemoteConnAllowed.x86=CD7B0
bMultimonAllowed.x86  =CD7B4
ulMaxDebugSessions.x86=CD7B8
bFUSEnabled.x86       =CD7BC
bInitialized.x64      =ECAB4
bServerSku.x64        =ECAB8
lMaxUserSessions.x64  =ECABC
bAppServerAllowed.x64 =ECAC4
bRemoteConnAllowed.x64=ECAC8
bMultimonAllowed.x64  =ECACC
ulMaxDebugSessions.x64=ECAD0
bFUSEnabled.x64       =ECAD4

[10.0.17763.1613-SLInit]
bInitialized.x86      =D3828
bServerSku.x86        =D382C
lMaxUserSessions.x86  =D3830
bAppServerAllowed.x86 =D3838
bRemoteConnAllowed.x86=D383C
bMultimonAllowed.x86  =D3840
ulMaxDebugSessions.x86=D3844
bFUSEnabled.x86       =D3848
bServerSku.x64        =F3B90
lMaxUserSessions.x64  =F3B94
bAppServerAllowed.x64 =F3B9C
bInitialized.x64      =F3B8C
bRemoteConnAllowed.x64=F3BA0
bMultimonAllowed.x64  =F3BA4
ulMaxDebugSessions.x64=F3BA8
bFUSEnabled.x64       =F3BAC

[10.0.17763.1697-SLInit]
bInitialized.x86      =D1828
bServerSku.x86        =D182C
lMaxUserSessions.x86  =D1830
bAppServerAllowed.x86 =D1838
bRemoteConnAllowed.x86=D183C
bMultimonAllowed.x86  =D1840
ulMaxDebugSessions.x86=D1844
bFUSEnabled.x86       =D1848
bInitialized.x64      =F3B8C
bServerSku.x64        =F3B90
lMaxUserSessions.x64  =F3B94
bAppServerAllowed.x64 =F3B9C
bRemoteConnAllowed.x64=F3BA0
bMultimonAllowed.x64  =F3BA4
ulMaxDebugSessions.x64=F3BA8
bFUSEnabled.x64       =F3BAC

[10.0.17763.1971-SLInit]
bInitialized.x64      =ECAB4
bServerSku.x64        =ECAB8
lMaxUserSessions.x64  =ECABC
bAppServerAllowed.x64 =ECAC4
bRemoteConnAllowed.x64=ECAC8
bMultimonAllowed.x64  =ECACC
ulMaxDebugSessions.x64=ECAD0
bFUSEnabled.x64       =ECAD4
bInitialized.x86      =CC79C
bServerSku.x86        =CC7A0
lMaxUserSessions.x86  =CC7A4
bAppServerAllowed.x86 =CC7AC
bRemoteConnAllowed.x86=CC7B0
bMultimonAllowed.x86  =CC7B4
ulMaxDebugSessions.x86=CC7B8
bFUSEnabled.x86       =CC7BC

[10.0.17763.2213-SLInit]
bInitialized.x64      =F3AC4
bServerSku.x64        =F3AC8
lMaxUserSessions.x64  =F3ACC
bAppServerAllowed.x64 =F3AD4
bRemoteConnAllowed.x64=F3AD8
bMultimonAllowed.x64  =F3ADC
ulMaxDebugSessions.x64=F3AE0
bFUSEnabled.x64       =F3AE4
bInitialized.x86      =D17BC
bServerSku.x86        =D17C0
lMaxUserSessions.x86  =D17C4
bAppServerAllowed.x86 =D17CC
bRemoteConnAllowed.x86=D17D0
bMultimonAllowed.x86  =D17D4
ulMaxDebugSessions.x86=D17D8
bFUSEnabled.x86       =D17DC

[10.0.17763.2268-SLInit]
bInitialized.x64      =F3AC4
bServerSku.x64        =F3AC8
lMaxUserSessions.x64  =F3ACC
bAppServerAllowed.x64 =F3AD4
bRemoteConnAllowed.x64=F3AD8
bMultimonAllowed.x64  =F3ADC
ulMaxDebugSessions.x64=F3AE0
bFUSEnabled.x64       =F3AE4
bInitialized.x86      =D17BC
bServerSku.x86        =D17C0
lMaxUserSessions.x86  =D17C4
bAppServerAllowed.x86 =D17CC
bRemoteConnAllowed.x86=D17D0
bMultimonAllowed.x86  =D17D4
ulMaxDebugSessions.x86=D17D8
bFUSEnabled.x86       =D17DC

[10.0.17763.2300-SLInit]
bInitialized.x64      =F3AC4
bServerSku.x64        =F3AC8
lMaxUserSessions.x64  =F3ACC
bAppServerAllowed.x64 =F3AD4
bRemoteConnAllowed.x64=F3AD8
bMultimonAllowed.x64  =F3ADC
ulMaxDebugSessions.x64=F3AE0
bFUSEnabled.x64       =F3AE4
bInitialized.x86      =D17BC
bServerSku.x86        =D17C0
lMaxUserSessions.x86  =D17C4
bAppServerAllowed.x86 =D17CC
bRemoteConnAllowed.x86=D17D0
bMultimonAllowed.x86  =D17D4
ulMaxDebugSessions.x86=D17D8
bFUSEnabled.x86       =D17DC

[10.0.17763.2628-SLInit]
bInitialized.x64      =F3B8C
bServerSku.x64        =F3B90
lMaxUserSessions.x64  =F3B94
bAppServerAllowed.x64 =F3B9C
bRemoteConnAllowed.x64=F3BA0
bMultimonAllowed.x64  =F3BA4
ulMaxDebugSessions.x64=F3BA8
bFUSEnabled.x64       =F3BAC

[10.0.17763.2931-SLInit]
bInitialized.x64      =F3B8C
bServerSku.x64        =F3B90
lMaxUserSessions.x64  =F3B94
bAppServerAllowed.x64 =F3B9C
bRemoteConnAllowed.x64=F3BA0
bMultimonAllowed.x64  =F3BA4
ulMaxDebugSessions.x64=F3BA8
bFUSEnabled.x64       =F3BAC

[10.0.17763.2989-SLInit]
bInitialized.x64      =114D1C
bServerSku.x64        =114D20
lMaxUserSessions.x64  =114D24
bAppServerAllowed.x64 =114D2C
bRemoteConnAllowed.x64=114D30
bMultimonAllowed.x64  =114D34
ulMaxDebugSessions.x64=114D38
bFUSEnabled.x64       =114D3C

[10.0.17763.3113-SLInit]
bInitialized.x64      =114D1C
bServerSku.x64        =114D20
lMaxUserSessions.x64  =114D24
bAppServerAllowed.x64 =114D2C
bRemoteConnAllowed.x64=114D30
bMultimonAllowed.x64  =114D34
ulMaxDebugSessions.x64=114D38
bFUSEnabled.x64       =114D3C

[10.0.17763.3232-SLInit]
bInitialized.x64      =115D1C
bServerSku.x64        =115D20
lMaxUserSessions.x64  =115D24
bAppServerAllowed.x64 =115D2C
bRemoteConnAllowed.x64=115D30
bMultimonAllowed.x64  =115D34
ulMaxDebugSessions.x64=115D38
bFUSEnabled.x64       =115D3C

[10.0.18252.1000-SLInit]
bInitialized.x64      =ECAB0
bServerSku.x64        =ECAB4
lMaxUserSessions.x64  =ECAB8
bAppServerAllowed.x64 =ECAC0
bRemoteConnAllowed.x64=ECAC4
bMultimonAllowed.x64  =ECAC8
ulMaxDebugSessions.x64=ECACC
bFUSEnabled.x64       =ECAD0

[10.0.18362.1-SLInit]
bInitialized.x86      =D477C
bServerSku.x86        =D4780
lMaxUserSessions.x86  =D4784
bAppServerAllowed.x86 =D478C
bRemoteConnAllowed.x86=D4790
bMultimonAllowed.x86  =D4794
ulMaxDebugSessions.x86=D4798
bFUSEnabled.x86       =D479C
bInitialized.x64      =F6A8C
bServerSku.x64        =F6A90
lMaxUserSessions.x64  =F6A94
bAppServerAllowed.x64 =F6A9C
bRemoteConnAllowed.x64=F6AA0
bMultimonAllowed.x64  =F6AA4
ulMaxDebugSessions.x64=F6AA8
bFUSEnabled.x64       =F6AAC

[10.0.18362.53-SLInit]
bInitialized.x86      =D577C
bServerSku.x86        =D5780
lMaxUserSessions.x86  =D5784
bAppServerAllowed.x86 =D578C
bRemoteConnAllowed.x86=D5790
bMultimonAllowed.x86  =D5794
ulMaxDebugSessions.x86=D5798
bFUSEnabled.x86       =D579C
bInitialized.x64      =F6A8C
bServerSku.x64        =F6A90
lMaxUserSessions.x64  =F6A94
bAppServerAllowed.x64 =F6A9C
bRemoteConnAllowed.x64=F6AA0
bMultimonAllowed.x64  =F6AA4
ulMaxDebugSessions.x64=F6AA8
bFUSEnabled.x64       =F6AAC

[10.0.18362.267-SLInit]
bInitialized.x86      =D577C
bServerSku.x86        =D5780
lMaxUserSessions.x86  =D5784
bAppServerAllowed.x86 =D578C
bRemoteConnAllowed.x86=D5790
bMultimonAllowed.x86  =D5794
ulMaxDebugSessions.x86=D5798
bFUSEnabled.x86       =D579C
bInitialized.x64      =F6A8C
bServerSku.x64        =F6A90
lMaxUserSessions.x64  =F6A94
bAppServerAllowed.x64 =F6A9C
bRemoteConnAllowed.x64=F6AA0
bMultimonAllowed.x64  =F6AA4
ulMaxDebugSessions.x64=F6AA8
bFUSEnabled.x64       =F6AAC

[10.0.18362.657-SLInit]
bInitialized.x86      =D577C
bServerSku.x86        =D5780
lMaxUserSessions.x86  =D5784
bAppServerAllowed.x86 =D578C
bRemoteConnAllowed.x86=D5790
bMultimonAllowed.x86  =D5794
ulMaxDebugSessions.x86=D5798
bFUSEnabled.x86       =D579C
bInitialized.x64      =F6A8C
bServerSku.x64        =F6A90
lMaxUserSessions.x64  =F6A94
bAppServerAllowed.x64 =F6A9C
bRemoteConnAllowed.x64=F6AA0
bMultimonAllowed.x64  =F6AA4
ulMaxDebugSessions.x64=F6AA8
bFUSEnabled.x64       =F6AAC

[10.0.18362.836-SLInit]
bInitialized.x86      =D577C
bServerSku.x86        =D5780
lMaxUserSessions.x86  =D5784
bAppServerAllowed.x86 =D578C
bRemoteConnAllowed.x86=D5790
bMultimonAllowed.x86  =D5794
ulMaxDebugSessions.x86=D5798
bFUSEnabled.x86       =D579C
bInitialized.x64      =F6A8C
bServerSku.x64        =F6A90
lMaxUserSessions.x64  =F6A94
bAppServerAllowed.x64 =F6A9C
bRemoteConnAllowed.x64=F6AA0
bMultimonAllowed.x64  =F6AA4
ulMaxDebugSessions.x64=F6AA8
bFUSEnabled.x64       =F6AAC

[10.0.18362.1316-SLInit]
bInitialized.x86      =D377C
bServerSku.x86        =D3780
lMaxUserSessions.x86  =D3784
bAppServerAllowed.x86 =D378C
bRemoteConnAllowed.x86=D3790
bMultimonAllowed.x86  =D3794
ulMaxDebugSessions.x86=D3798
bFUSEnabled.x86       =D379C
bInitialized.x64      =F6A8C
bServerSku.x64        =F6A90
lMaxUserSessions.x64  =F6A94
bAppServerAllowed.x64 =F6A9C
bRemoteConnAllowed.x64=F6AA0
bMultimonAllowed.x64  =F6AA4
ulMaxDebugSessions.x64=F6AA8
bFUSEnabled.x64       =F6AAC

[10.0.18362.1533-SLInit]
bInitialized.x64      =F6A8C
bServerSku.x64        =F6A90
lMaxUserSessions.x64  =F6A94
bAppServerAllowed.x64 =F6A9C
bRemoteConnAllowed.x64=F6AA0
bMultimonAllowed.x64  =F6AA4
ulMaxDebugSessions.x64=F6AA8
bFUSEnabled.x64       =F6AAC

[10.0.18362.2158-SLInit]
bInitialized.x64      =F6A8C
bServerSku.x64        =F6A90
lMaxUserSessions.x64  =F6A94
bAppServerAllowed.x64 =F6A9C
bRemoteConnAllowed.x64=F6AA0
bMultimonAllowed.x64  =F6AA4
ulMaxDebugSessions.x64=F6AA8
bFUSEnabled.x64       =F6AAC

[10.0.18362.1766-SLInit]
bInitialized.x64      =F6A8C
bServerSku.x64        =F6A90
lMaxUserSessions.x64  =F6A94
bAppServerAllowed.x64 =F6A9C
bRemoteConnAllowed.x64=F6AA0
bMultimonAllowed.x64  =F6AA4
ulMaxDebugSessions.x64=F6AA8
bFUSEnabled.x64       =F6AAC

[10.0.18362.1916-SLInit]
bInitialized.x64      =F6A8C
bServerSku.x64        =F6A90
lMaxUserSessions.x64  =F6A94
bAppServerAllowed.x64 =F6A9C
bRemoteConnAllowed.x64=F6AA0
bMultimonAllowed.x64  =F6AA4
ulMaxDebugSessions.x64=F6AA8
bFUSEnabled.x64       =F6AAC

[10.0.18963.1000-SLInit]
bInitialized.x64      =102DD8
bServerSku.x64        =102DDC
lMaxUserSessions.x64  =102DE0
bAppServerAllowed.x64 =102DE8
bRemoteConnAllowed.x64=102DF0
bMultimonAllowed.x64  =102DF4
ulMaxDebugSessions.x64=102DF8
bFUSEnabled.x64       =102DFC

[10.0.19041.1-SLInit]
bInitialized.x64      =103FF8
bServerSku.x64        =103FFC
lMaxUserSessions.x64  =104000
bAppServerAllowed.x64 =104008
bRemoteConnAllowed.x64=104010
bMultimonAllowed.x64  =104014
ulMaxDebugSessions.x64=104018
bFUSEnabled.x64       =10401C

[10.0.19041.84-SLInit]
bInitialized.x86      =CF920
bServerSku.x86        =CF924
lMaxUserSessions.x86  =CF928
bAppServerAllowed.x86 =CF930
bRemoteConnAllowed.x86=CF938
bMultimonAllowed.x86  =CF93C
ulMaxDebugSessions.x86=CF940
bFUSEnabled.x86       =CF944
bInitialized.x64      =103FF8
bServerSku.x64        =103FFC
lMaxUserSessions.x64  =104000
bAppServerAllowed.x64 =104008
bRemoteConnAllowed.x64=104010
bMultimonAllowed.x64  =104014
ulMaxDebugSessions.x64=104018
bFUSEnabled.x64       =10401C

[10.0.19041.662-SLInit]
bInitialized.x86      =D1954
bServerSku.x86        =D1958
lMaxUserSessions.x86  =D195C
bAppServerAllowed.x86 =D1964
bRemoteConnAllowed.x86=D196C
bMultimonAllowed.x86  =D1970
ulMaxDebugSessions.x86=D1974
bFUSEnabled.x86       =D1978
bInitialized.x64      =106028
bServerSku.x64        =10602C
lMaxUserSessions.x64  =106030
bAppServerAllowed.x64 =106038
bRemoteConnAllowed.x64=106040
bMultimonAllowed.x64  =106044
ulMaxDebugSessions.x64=106048
bFUSEnabled.x64       =10604C

[10.0.19041.746-SLInit]
bInitialized.x86      =D0954
bServerSku.x86        =D0958
lMaxUserSessions.x86  =D095C
bAppServerAllowed.x86 =D0964
bRemoteConnAllowed.x86=D096C
bMultimonAllowed.x86  =D0970
ulMaxDebugSessions.x86=D0974
bFUSEnabled.x86       =D0978
bInitialized.x64      =106028
bServerSku.x64        =10602C
lMaxUserSessions.x64  =106030
bAppServerAllowed.x64 =106038
bRemoteConnAllowed.x64=106040
bMultimonAllowed.x64  =106044
ulMaxDebugSessions.x64=106048
bFUSEnabled.x64       =10604C

[10.0.19041.782-SLInit]
bInitialized.x64      =106028
bServerSku.x64        =10602C
lMaxUserSessions.x64  =106030
bAppServerAllowed.x64 =106038
bRemoteConnAllowed.x64=106040
bMultimonAllowed.x64  =106044
ulMaxDebugSessions.x64=106048
bFUSEnabled.x64       =10604C

[10.0.19041.789-SLInit]
bInitialized.x86      =D0954
bServerSku.x86        =D0958
lMaxUserSessions.x86  =D095C
bAppServerAllowed.x86 =D0964
bRemoteConnAllowed.x86=D096C
bMultimonAllowed.x86  =D0970
ulMaxDebugSessions.x86=D0974
bFUSEnabled.x86       =D0978
bInitialized.x64      =106028
bServerSku.x64        =10602C
lMaxUserSessions.x64  =106030
bAppServerAllowed.x64 =106038
bRemoteConnAllowed.x64=106040
bMultimonAllowed.x64  =106044
ulMaxDebugSessions.x64=106048
bFUSEnabled.x64       =10604C

[10.0.19041.962-SLInit]
bInitialized.x64      =107108
bServerSku.x64        =10710C
lMaxUserSessions.x64  =107110
bAppServerAllowed.x64 =107118
bRemoteConnAllowed.x64=107120
bMultimonAllowed.x64  =107124
ulMaxDebugSessions.x64=107128
bFUSEnabled.x64       =10712C

[10.0.19041.964-SLInit]
bInitialized.x86      =D1A04
bServerSku.x86        =D1A08
lMaxUserSessions.x86  =D1A0C
bAppServerAllowed.x86 =D1A14
bRemoteConnAllowed.x86=D1A1C
bMultimonAllowed.x86  =D1A20
ulMaxDebugSessions.x86=D1A24
bFUSEnabled.x86       =D1A28
bInitialized.x64      =107108
bServerSku.x64        =10710C
lMaxUserSessions.x64  =107110
bAppServerAllowed.x64 =107118
bRemoteConnAllowed.x64=107120
bMultimonAllowed.x64  =107124
ulMaxDebugSessions.x64=107128
bFUSEnabled.x64       =10712C

[10.0.19041.1023-SLInit]
bInitialized.x64      =107108
bServerSku.x64        =10710C
lMaxUserSessions.x64  =107110
bAppServerAllowed.x64 =107118
bRemoteConnAllowed.x64=107120
bMultimonAllowed.x64  =107124
ulMaxDebugSessions.x64=107128
bFUSEnabled.x64       =10712C

[10.0.19041.1081-SLInit]
bInitialized.x64      =107108
bServerSku.x64        =10710C
lMaxUserSessions.x64  =107110
bAppServerAllowed.x64 =107118
bRemoteConnAllowed.x64=107120
bMultimonAllowed.x64  =107124
ulMaxDebugSessions.x64=107128
bFUSEnabled.x64       =10712C
bInitialized.x86      =D1A04
bServerSku.x86        =D1A08
lMaxUserSessions.x86  =D1A0C
bAppServerAllowed.x86 =D1A14
bRemoteConnAllowed.x86=D1A1C
bMultimonAllowed.x86  =D1A20
ulMaxDebugSessions.x86=D1A24
bFUSEnabled.x86       =D1A28

[10.0.19041.1200-SLInit]
bInitialized.x64      =107108
bServerSku.x64        =10710C
lMaxUserSessions.x64  =107110
bAppServerAllowed.x64 =107118
bRemoteConnAllowed.x64=107120
bMultimonAllowed.x64  =107124
ulMaxDebugSessions.x64=107128
bFUSEnabled.x64       =10712C

[10.0.19041.1202-SLInit]
bInitialized.x86      =D1A04
bServerSku.x86        =D1A08
lMaxUserSessions.x86  =D1A0C
bAppServerAllowed.x86 =D1A14
bRemoteConnAllowed.x86=D1A1C
bMultimonAllowed.x86  =D1A20
ulMaxDebugSessions.x86=D1A24
bFUSEnabled.x86       =D1A28
bInitialized.x64      =107108
bServerSku.x64        =10710C
lMaxUserSessions.x64  =107110
bAppServerAllowed.x64 =107118
bRemoteConnAllowed.x64=107120
bMultimonAllowed.x64  =107124
ulMaxDebugSessions.x64=107128
bFUSEnabled.x64       =10712C

[10.0.19041.1319-SLInit]
bInitialized.x64      =107108
bServerSku.x64        =10710C
lMaxUserSessions.x64  =107110
bAppServerAllowed.x64 =107118
bRemoteConnAllowed.x64=107120
bMultimonAllowed.x64  =107124
ulMaxDebugSessions.x64=107128
bFUSEnabled.x64       =10712C

[10.0.19041.1320-SLInit]
bInitialized.x64      =107108
bServerSku.x64        =10710C
lMaxUserSessions.x64  =107110
bAppServerAllowed.x64 =107118
bRemoteConnAllowed.x64=107120
bMultimonAllowed.x64  =107124
ulMaxDebugSessions.x64=107128
bFUSEnabled.x64       =10712C
bInitialized.x86      =D1A04
bServerSku.x86        =D1A08
lMaxUserSessions.x86  =D1A0C
bAppServerAllowed.x86 =D1A14
bRemoteConnAllowed.x86=D1A1C
bMultimonAllowed.x86  =D1A20
ulMaxDebugSessions.x86=D1A24
bFUSEnabled.x86       =D1A28

[10.0.19041.1348-SLInit]
bInitialized.x64      =107108
bServerSku.x64        =10710C
lMaxUserSessions.x64  =107110
bAppServerAllowed.x64 =107118
bRemoteConnAllowed.x64=107120
bMultimonAllowed.x64  =107124
ulMaxDebugSessions.x64=107128
bFUSEnabled.x64       =10712C
bInitialized.x86      =D1A04
bServerSku.x86        =D1A08
lMaxUserSessions.x86  =D1A0C
bAppServerAllowed.x86 =D1A14
bRemoteConnAllowed.x86=D1A1C
bMultimonAllowed.x86  =D1A20
ulMaxDebugSessions.x86=D1A24
bFUSEnabled.x86       =D1A28

[10.0.19041.1379-SLInit]
bInitialized.x64      =107108
bServerSku.x64        =10710C
lMaxUserSessions.x64  =107110
bAppServerAllowed.x64 =107118
bRemoteConnAllowed.x64=107120
bMultimonAllowed.x64  =107124
ulMaxDebugSessions.x64=107128
bFUSEnabled.x64       =10712C

[10.0.19041.1381-SLInit]
bInitialized.x64      =107108
bServerSku.x64        =10710C
lMaxUserSessions.x64  =107110
bAppServerAllowed.x64 =107118
bRemoteConnAllowed.x64=107120
bMultimonAllowed.x64  =107124
ulMaxDebugSessions.x64=107128
bFUSEnabled.x64       =10712C

[10.0.19041.1387-SLInit]
bInitialized.x64      =107108
bServerSku.x64        =10710C
lMaxUserSessions.x64  =107110
bAppServerAllowed.x64 =107118
bRemoteConnAllowed.x64=107120
bMultimonAllowed.x64  =107124
ulMaxDebugSessions.x64=107128
bFUSEnabled.x64       =10712C
bInitialized.x86      =D1A04
bServerSku.x86        =D1A08
lMaxUserSessions.x86  =D1A0C
bAppServerAllowed.x86 =D1A14
bRemoteConnAllowed.x86=D1A1C
bMultimonAllowed.x86  =D1A20
ulMaxDebugSessions.x86=D1A24
bFUSEnabled.x86       =D1A28

[10.0.19041.1499-SLInit]
bInitialized.x64      =106028
bServerSku.x64        =10602C
lMaxUserSessions.x64  =106030
bAppServerAllowed.x64 =106038
bRemoteConnAllowed.x64=106040
bMultimonAllowed.x64  =106044
ulMaxDebugSessions.x64=106048
bFUSEnabled.x64       =10604C

[10.0.19041.1503-SLInit]
bInitialized.x86      =D1954
bServerSku.x86        =D1958
lMaxUserSessions.x86  =D195C
bAppServerAllowed.x86 =D1964
bRemoteConnAllowed.x86=D196C
bMultimonAllowed.x86  =D1970
ulMaxDebugSessions.x86=D1974
bFUSEnabled.x86       =D1978
bInitialized.x64      =106028
bServerSku.x64        =10602C
lMaxUserSessions.x64  =106030
bAppServerAllowed.x64 =106038
bRemoteConnAllowed.x64=106040
bMultimonAllowed.x64  =106044
ulMaxDebugSessions.x64=106048
bFUSEnabled.x64       =10604C

[10.0.19041.1561-SLInit]
bInitialized.x86      =CF920
bServerSku.x86        =CF924
lMaxUserSessions.x86  =CF928
bAppServerAllowed.x86 =CF930
bRemoteConnAllowed.x86=CF938
bMultimonAllowed.x86  =CF93C
ulMaxDebugSessions.x86=CF940
bFUSEnabled.x86       =CF944
bInitialized.x64      =104FF8
bServerSku.x64        =104FFC
lMaxUserSessions.x64  =105000
bAppServerAllowed.x64 =105008
bRemoteConnAllowed.x64=105010
bMultimonAllowed.x64  =105014
ulMaxDebugSessions.x64=105018
bFUSEnabled.x64       =10501C

[10.0.19041.1566-SLInit]
bInitialized.x86      =CF920
bServerSku.x86        =CF924
lMaxUserSessions.x86  =CF928
bAppServerAllowed.x86 =CF930
bRemoteConnAllowed.x86=CF938
bMultimonAllowed.x86  =CF93C
ulMaxDebugSessions.x86=CF940
bFUSEnabled.x86       =CF944
bInitialized.x64      =104FF8
bServerSku.x64        =104FFC
lMaxUserSessions.x64  =105000
bAppServerAllowed.x64 =105008
bRemoteConnAllowed.x64=105010
bMultimonAllowed.x64  =105014
ulMaxDebugSessions.x64=105018
bFUSEnabled.x64       =10501C

[10.0.19041.1618-SLInit]
bInitialized.x64      =104FF8
bServerSku.x64        =104FFC
lMaxUserSessions.x64  =105000
bAppServerAllowed.x64 =105008
bRemoteConnAllowed.x64=105010
bMultimonAllowed.x64  =105014
ulMaxDebugSessions.x64=105018
bFUSEnabled.x64       =10501C

[10.0.19041.1620-SLInit]
bInitialized.x86      =CF920
bServerSku.x86        =CF924
lMaxUserSessions.x86  =CF928
bAppServerAllowed.x86 =CF930
bRemoteConnAllowed.x86=CF938
bMultimonAllowed.x86  =CF93C
ulMaxDebugSessions.x86=CF940
bFUSEnabled.x86       =CF944
bInitialized.x64      =104FF8
bServerSku.x64        =104FFC
lMaxUserSessions.x64  =105000
bAppServerAllowed.x64 =105008
bRemoteConnAllowed.x64=105010
bMultimonAllowed.x64  =105014
ulMaxDebugSessions.x64=105018
bFUSEnabled.x64       =10501C

[10.0.19041.1679-SLInit]
bInitialized.x64      =1070F8
bServerSku.x64        =1070FC
lMaxUserSessions.x64  =107100
bAppServerAllowed.x64 =107108
bRemoteConnAllowed.x64=107110
bMultimonAllowed.x64  =107114
ulMaxDebugSessions.x64=107118
bFUSEnabled.x64       =10711C

[10.0.19041.1682-SLInit]
bInitialized.x86      =D19E0
bServerSku.x86        =D19E4
lMaxUserSessions.x86  =D19E8
bAppServerAllowed.x86 =D19F0
bRemoteConnAllowed.x86=D19F8
bMultimonAllowed.x86  =D19FC
ulMaxDebugSessions.x86=D1A00
bFUSEnabled.x86       =D1A04
bInitialized.x64      =1070F8
bServerSku.x64        =1070FC
lMaxUserSessions.x64  =107100
bAppServerAllowed.x64 =107108
bRemoteConnAllowed.x64=107110
bMultimonAllowed.x64  =107114
ulMaxDebugSessions.x64=107118
bFUSEnabled.x64       =10711C

[10.0.19041.1737-SLInit]
bInitialized.x64      =127164
bServerSku.x64        =127168
lMaxUserSessions.x64  =12716C
bAppServerAllowed.x64 =127174
bRemoteConnAllowed.x64=12717C
bMultimonAllowed.x64  =127180
ulMaxDebugSessions.x64=127184
bFUSEnabled.x64       =127188

[10.0.19041.1739-SLInit]
bInitialized.x64      =127164
bServerSku.x64        =127168
lMaxUserSessions.x64  =12716C
bAppServerAllowed.x64 =127174
bRemoteConnAllowed.x64=12717C
bMultimonAllowed.x64  =127180
ulMaxDebugSessions.x64=127184
bFUSEnabled.x64       =127188

[10.0.19041.1741-SLInit]
bInitialized.x86      =E5A2C
bServerSku.x86        =E5A30
lMaxUserSessions.x86  =E5A34
bAppServerAllowed.x86 =E5A3C
bRemoteConnAllowed.x86=E5A44
bMultimonAllowed.x86  =E5A48
ulMaxDebugSessions.x86=E5A4C
bFUSEnabled.x86       =E5A50
bInitialized.x64      =127164
bServerSku.x64        =127168
lMaxUserSessions.x64  =12716C
bAppServerAllowed.x64 =127174
bRemoteConnAllowed.x64=12717C
bMultimonAllowed.x64  =127180
ulMaxDebugSessions.x64=127184
bFUSEnabled.x64       =127188

[10.0.19613.1000-SLInit]
bInitialized.x64      =117040
bServerSku.x64        =117044
lMaxUserSessions.x64  =117048
bAppServerAllowed.x64 =117050
bRemoteConnAllowed.x64=117058
bMultimonAllowed.x64  =11705C
ulMaxDebugSessions.x64=117060
bFUSEnabled.x64       =117064

[10.0.19619.1000-SLInit]
bInitialized.x64      =117040
bServerSku.x64        =117044
lMaxUserSessions.x64  =117048
bAppServerAllowed.x64 =117050
bRemoteConnAllowed.x64=117058
bMultimonAllowed.x64  =11705C
ulMaxDebugSessions.x64=117060
bFUSEnabled.x64       =117064

[10.0.19628.1-SLInit]
bInitialized.x64      =118030
bServerSku.x64        =118034
lMaxUserSessions.x64  =118038
bAppServerAllowed.x64 =118040
bRemoteConnAllowed.x64=118048
bMultimonAllowed.x64  =11804C
ulMaxDebugSessions.x64=118050
bFUSEnabled.x64       =118054

[10.0.19631.1-SLInit]
bInitialized.x64      =119030
bServerSku.x64        =119034
lMaxUserSessions.x64  =119038
bAppServerAllowed.x64 =119040
bRemoteConnAllowed.x64=119048
bMultimonAllowed.x64  =11904C
ulMaxDebugSessions.x64=119050
bFUSEnabled.x64       =119054

[10.0.19635.1-SLInit]
bInitialized.x64      =119030
bServerSku.x64        =119034
lMaxUserSessions.x64  =119038
bAppServerAllowed.x64 =119040
bRemoteConnAllowed.x64=119048
bMultimonAllowed.x64  =11904C
ulMaxDebugSessions.x64=119050
bFUSEnabled.x64       =119054

[10.0.19640.1-SLInit]
bInitialized.x64      =119030
bServerSku.x64        =119034
lMaxUserSessions.x64  =119038
bAppServerAllowed.x64 =119040
bRemoteConnAllowed.x64=119048
bMultimonAllowed.x64  =11904C
ulMaxDebugSessions.x64=119050
bFUSEnabled.x64       =119054

[10.0.19645.1-SLInit]
bInitialized.x64      =119030
bServerSku.x64        =119034
lMaxUserSessions.x64  =119038
bAppServerAllowed.x64 =119040
bRemoteConnAllowed.x64=119048
bMultimonAllowed.x64  =11904C
ulMaxDebugSessions.x64=119050
bFUSEnabled.x64       =119054

[10.0.20150.1000-SLInit]
bInitialized.x64      =11FEC8
bServerSku.x64        =11FECC
lMaxUserSessions.x64  =11FED0
bAppServerAllowed.x64 =11FED8
bRemoteConnAllowed.x64=11FEE0
bMultimonAllowed.x64  =11FEE4
ulMaxDebugSessions.x64=11FEE8
bFUSEnabled.x64       =11FEEC

[10.0.20152.1000-SLInit]
bInitialized.x64      =11FEC8
bServerSku.x64        =11FECC
lMaxUserSessions.x64  =11FED0
bAppServerAllowed.x64 =11FED8
bRemoteConnAllowed.x64=11FEE0
bMultimonAllowed.x64  =11FEE4
ulMaxDebugSessions.x64=11FEE8
bFUSEnabled.x64       =11FEEC

[10.0.20161.1000-SLInit]
bInitialized.x64      =11FEC8
bServerSku.x64        =11FECC
lMaxUserSessions.x64  =11FED0
bAppServerAllowed.x64 =11FED8
bRemoteConnAllowed.x64=11FEE0
bMultimonAllowed.x64  =11FEE4
ulMaxDebugSessions.x64=11FEEC
bFUSEnabled.x64       =11FEF0

[10.0.20170.1000-SLInit]
bInitialized.x64      =120EC8
bServerSku.x64        =120ECC
lMaxUserSessions.x64  =120ED0
bAppServerAllowed.x64 =120ED8
bRemoteConnAllowed.x64=120EE0
bMultimonAllowed.x64  =120EE4
ulMaxDebugSessions.x64=120EEC
bFUSEnabled.x64       =120EF0

[10.0.20175.1000-SLInit]
bInitialized.x64      =120EC8
bServerSku.x64        =120ECC
lMaxUserSessions.x64  =120ED0
bAppServerAllowed.x64 =120ED8
bRemoteConnAllowed.x64=120EE0
bMultimonAllowed.x64  =120EE4
ulMaxDebugSessions.x64=120EEC
bFUSEnabled.x64       =120EF0

[10.0.20180.1000-SLInit]
bInitialized.x64      =11DF18
bServerSku.x64        =11DF1C
lMaxUserSessions.x64  =11DF20
bAppServerAllowed.x64 =11DF28
bRemoteConnAllowed.x64=11DF30
bMultimonAllowed.x64  =11DF34
ulMaxDebugSessions.x64=11DF3C
bFUSEnabled.x64       =11DF40

[10.0.20185.1000-SLInit]
bInitialized.x64      =11DF18
bServerSku.x64        =11DF1C
lMaxUserSessions.x64  =11DF20
bAppServerAllowed.x64 =11DF28
bRemoteConnAllowed.x64=11DF30
bMultimonAllowed.x64  =11DF34
ulMaxDebugSessions.x64=11DF3C
bFUSEnabled.x64       =11DF40

[10.0.20190.1000-SLInit]
bInitialized.x64      =11DF18
bServerSku.x64        =11DF1C
lMaxUserSessions.x64  =11DF20
bAppServerAllowed.x64 =11DF28
bRemoteConnAllowed.x64=11DF30
bMultimonAllowed.x64  =11DF34
ulMaxDebugSessions.x64=11DF3C
bFUSEnabled.x64       =11DF40

[10.0.20197.1000-SLInit]
bInitialized.x64      =11DF18
bServerSku.x64        =11DF1C
lMaxUserSessions.x64  =11DF20
bAppServerAllowed.x64 =11DF28
bRemoteConnAllowed.x64=11DF30
bMultimonAllowed.x64  =11DF34
ulMaxDebugSessions.x64=11DF3C
bFUSEnabled.x64       =11DF40

[10.0.20201.1000-SLInit]
bInitialized.x64      =11FF18
bServerSku.x64        =11FF1C
lMaxUserSessions.x64  =11FF20
bAppServerAllowed.x64 =11FF28
bRemoteConnAllowed.x64=11FF30
bMultimonAllowed.x64  =11FF34
ulMaxDebugSessions.x64=11FF3C
bFUSEnabled.x64       =11FF40

[10.0.20206.1000-SLInit]
bInitialized.x64      =11FF0C
bServerSku.x64        =11FF10
lMaxUserSessions.x64  =11FF14
bAppServerAllowed.x64 =11FF1C
bRemoteConnAllowed.x64=11FF24
bMultimonAllowed.x64  =11FF28
ulMaxDebugSessions.x64=11FF30
bFUSEnabled.x64       =11FF34

[10.0.20211.1000-SLInit]
bInitialized.x64      =11FF0C
bServerSku.x64        =11FF10
lMaxUserSessions.x64  =11FF14
bAppServerAllowed.x64 =11FF1C
bRemoteConnAllowed.x64=11FF24
bMultimonAllowed.x64  =11FF28
ulMaxDebugSessions.x64=11FF30
bFUSEnabled.x64       =11FF34

[10.0.20215.1000-SLInit]
bInitialized.x64      =11FF0C
bServerSku.x64        =11FF10
lMaxUserSessions.x64  =11FF14
bAppServerAllowed.x64 =11FF1C
bRemoteConnAllowed.x64=11FF24
bMultimonAllowed.x64  =11FF28
ulMaxDebugSessions.x64=11FF30
bFUSEnabled.x64       =11FF34

[10.0.20221.1000-SLInit]
bInitialized.x64      =11FE9C
bServerSku.x64        =11FEA0
lMaxUserSessions.x64  =11FEA4
bAppServerAllowed.x64 =11FEAC
bRemoteConnAllowed.x64=11FEB4
bMultimonAllowed.x64  =11FEB8
ulMaxDebugSessions.x64=11FEC0
bFUSEnabled.x64       =11FEC4

[10.0.20226.1000-SLInit]
bInitialized.x64      =11FE9C
bServerSku.x64        =11FEA0
lMaxUserSessions.x64  =11FEA4
bAppServerAllowed.x64 =11FEAC
bRemoteConnAllowed.x64=11FEB4
bMultimonAllowed.x64  =11FEB8
ulMaxDebugSessions.x64=11FEC0
bFUSEnabled.x64       =11FEC4

[10.0.20231.1000-SLInit]
bInitialized.x64      =11FE9C
bServerSku.x64        =11FEA0
lMaxUserSessions.x64  =11FEA4
bAppServerAllowed.x64 =11FEAC
bRemoteConnAllowed.x64=11FEB4
bMultimonAllowed.x64  =11FEB8
ulMaxDebugSessions.x64=11FEC0
bFUSEnabled.x64       =11FEC4

[10.0.20236.1000-SLInit]
bInitialized.x64      =11FE9C
bServerSku.x64        =11FEA0
lMaxUserSessions.x64  =11FEA4
bAppServerAllowed.x64 =11FEAC
bRemoteConnAllowed.x64=11FEB4
bMultimonAllowed.x64  =11FEB8
ulMaxDebugSessions.x64=11FEC0
bFUSEnabled.x64       =11FEC4

[10.0.20241.1000-SLInit]
bInitialized.x64      =11EE9C
bServerSku.x64        =11EEA0
lMaxUserSessions.x64  =11EEA4
bAppServerAllowed.x64 =11EEAC
bRemoteConnAllowed.x64=11EEB4
bMultimonAllowed.x64  =11EEB8
ulMaxDebugSessions.x64=11EEC0
bFUSEnabled.x64       =11EEC4

[10.0.20246.1-SLInit]
bInitialized.x64      =11EE9C
bServerSku.x64        =11EEA0
lMaxUserSessions.x64  =11EEA4
bAppServerAllowed.x64 =11EEAC
bRemoteConnAllowed.x64=11EEB4
bMultimonAllowed.x64  =11EEB8
ulMaxDebugSessions.x64=11EEC0
bFUSEnabled.x64       =11EEC4

[10.0.20251.1-SLInit]
bInitialized.x64      =11EE9C
bServerSku.x64        =11EEA0
lMaxUserSessions.x64  =11EEA4
bAppServerAllowed.x64 =11EEAC
bRemoteConnAllowed.x64=11EEB4
bMultimonAllowed.x64  =11EEB8
ulMaxDebugSessions.x64=11EEC0
bFUSEnabled.x64       =11EEC4

[10.0.20257.1-SLInit]
bInitialized.x64      =11EE9C
bServerSku.x64        =11EEA0
lMaxUserSessions.x64  =11EEA4
bAppServerAllowed.x64 =11EEAC
bRemoteConnAllowed.x64=11EEB4
bMultimonAllowed.x64  =11EEB8
ulMaxDebugSessions.x64=11EEC0
bFUSEnabled.x64       =11EEC4

[10.0.20262.1-SLInit]
bInitialized.x64      =11EE9C
bServerSku.x64        =11EEA0
lMaxUserSessions.x64  =11EEA4
bAppServerAllowed.x64 =11EEAC
bRemoteConnAllowed.x64=11EEB4
bMultimonAllowed.x64  =11EEB8
ulMaxDebugSessions.x64=11EEC0
bFUSEnabled.x64       =11EEC4

[10.0.20279.1-SLInit]
bInitialized.x64      =11EE9C
bServerSku.x64        =11EEA0
lMaxUserSessions.x64  =11EEA4
bAppServerAllowed.x64 =11EEAC
bRemoteConnAllowed.x64=11EEB4
bMultimonAllowed.x64  =11EEB8
ulMaxDebugSessions.x64=11EEC0
bFUSEnabled.x64       =11EEC4

[10.0.20348.143-SLInit]
bInitialized.x64      =11EEAC
bServerSku.x64        =11EEB0
lMaxUserSessions.x64  =11EEB4
bAppServerAllowed.x64 =11EEBC
bRemoteConnAllowed.x64=11EEC4
bMultimonAllowed.x64  =11EEC8
ulMaxDebugSessions.x64=11EED0
bFUSEnabled.x64       =11EED4

[10.0.20348.261-SLInit]
bInitialized.x64      =11EEAC
bServerSku.x64        =11EEB0
lMaxUserSessions.x64  =11EEB4
bAppServerAllowed.x64 =11EEBC
bRemoteConnAllowed.x64=11EEC4
bMultimonAllowed.x64  =11EEC8
ulMaxDebugSessions.x64=11EED0
bFUSEnabled.x64       =11EED4

[10.0.20348.350-SLInit]
bInitialized.x64      =11EEAC
bServerSku.x64        =11EEB0
lMaxUserSessions.x64  =11EEB4
bAppServerAllowed.x64 =11EEBC
bRemoteConnAllowed.x64=11EEC4
bMultimonAllowed.x64  =11EEC8
ulMaxDebugSessions.x64=11EED0
bFUSEnabled.x64       =11EED4

[10.0.20348.380-SLInit]
bInitialized.x64      =11EEAC
bServerSku.x64        =11EEB0
lMaxUserSessions.x64  =11EEB4
bAppServerAllowed.x64 =11EEBC
bRemoteConnAllowed.x64=11EEC4
bMultimonAllowed.x64  =11EEC8
ulMaxDebugSessions.x64=11EED0
bFUSEnabled.x64       =11EED4

[10.0.20348.502-SLInit]
bInitialized.x64      =11FEAC
bServerSku.x64        =11FEB0
lMaxUserSessions.x64  =11FEB4
bAppServerAllowed.x64 =11FEBC
bRemoteConnAllowed.x64=11FEC4
bMultimonAllowed.x64  =11FEC8
ulMaxDebugSessions.x64=11FED0
bFUSEnabled.x64       =11FED4

[10.0.20348.617-SLInit]
bInitialized.x64      =121FAC
bServerSku.x64        =121FB0
lMaxUserSessions.x64  =121FB4
bAppServerAllowed.x64 =121FBC
bRemoteConnAllowed.x64=121FC4
bMultimonAllowed.x64  =121FC8
ulMaxDebugSessions.x64=121FD0
bFUSEnabled.x64       =121FD4

[10.0.20348.681-SLInit]
bInitialized.x64      =121FAC
bServerSku.x64        =121FB0
lMaxUserSessions.x64  =121FB4
bAppServerAllowed.x64 =121FBC
bRemoteConnAllowed.x64=121FC4
bMultimonAllowed.x64  =121FC8
ulMaxDebugSessions.x64=121FD0
bFUSEnabled.x64       =121FD4

[10.0.20348.740-SLInit]
bInitialized.x64      =121FAC
bServerSku.x64        =121FB0
lMaxUserSessions.x64  =121FB4
bAppServerAllowed.x64 =121FBC
bRemoteConnAllowed.x64=121FC4
bMultimonAllowed.x64  =121FC8
ulMaxDebugSessions.x64=121FD0
bFUSEnabled.x64       =121FD4

[10.0.20348.859-SLInit]
bInitialized.x64      =121FAC
bServerSku.x64        =121FB0
lMaxUserSessions.x64  =121FB4
bAppServerAllowed.x64 =121FBC
bRemoteConnAllowed.x64=121FC4
bMultimonAllowed.x64  =121FC8
ulMaxDebugSessions.x64=121FD0
bFUSEnabled.x64       =121FD4

[10.0.21277.1000-SLInit]
bInitialized.x64      =11EE9C
bServerSku.x64        =11EEA0
lMaxUserSessions.x64  =11EEA4
bAppServerAllowed.x64 =11EEAC
bRemoteConnAllowed.x64=11EEB4
bMultimonAllowed.x64  =11EEB8
ulMaxDebugSessions.x64=11EEC0
bFUSEnabled.x64       =11EEC4

[10.0.21286.1000-SLInit]
bInitialized.x64      =11DE9C
bServerSku.x64        =11DEA0
lMaxUserSessions.x64  =11DEA4
bAppServerAllowed.x64 =11DEAC
bRemoteConnAllowed.x64=11DEB4
bMultimonAllowed.x64  =11DEB8
ulMaxDebugSessions.x64=11DEC0
bFUSEnabled.x64       =11DEC4

[10.0.21292.1000-SLInit]
bInitialized.x64      =11DE9C
bServerSku.x64        =11DEA0
lMaxUserSessions.x64  =11DEA4
bAppServerAllowed.x64 =11DEAC
bRemoteConnAllowed.x64=11DEB4
bMultimonAllowed.x64  =11DEB8
ulMaxDebugSessions.x64=11DEC0
bFUSEnabled.x64       =11DEC4

[10.0.21296.1000-SLInit]
bInitialized.x64      =11DE9C
bServerSku.x64        =11DEA0
lMaxUserSessions.x64  =11DEA4
bAppServerAllowed.x64 =11DEAC
bRemoteConnAllowed.x64=11DEB4
bMultimonAllowed.x64  =11DEB8
ulMaxDebugSessions.x64=11DEC0
bFUSEnabled.x64       =11DEC4

[10.0.21301.1000-SLInit]
bInitialized.x64      =11DE9C
bServerSku.x64        =11DEA0
lMaxUserSessions.x64  =11DEA4
bAppServerAllowed.x64 =11DEAC
bRemoteConnAllowed.x64=11DEB4
bMultimonAllowed.x64  =11DEB8
ulMaxDebugSessions.x64=11DEC0
bFUSEnabled.x64       =11DEC4

[10.0.21313.1000-SLInit]
bInitialized.x64      =11DE9C
bServerSku.x64        =11DEA0
lMaxUserSessions.x64  =11DEA4
bAppServerAllowed.x64 =11DEAC
bRemoteConnAllowed.x64=11DEB4
bMultimonAllowed.x64  =11DEB8
ulMaxDebugSessions.x64=11DEC0
bFUSEnabled.x64       =11DEC4

[10.0.21332.1000-SLInit]
bInitialized.x64      =11DE9C
bServerSku.x64        =11DEA0
lMaxUserSessions.x64  =11DEA4
bAppServerAllowed.x64 =11DEAC
bRemoteConnAllowed.x64=11DEB4
bMultimonAllowed.x64  =11DEB8
ulMaxDebugSessions.x64=11DEC0
bFUSEnabled.x64       =11DEC4

[10.0.21343.1000-SLInit]
bInitialized.x64      =11EECC
bServerSku.x64        =11EED0
lMaxUserSessions.x64  =11EED4
bAppServerAllowed.x64 =11EEDC
bRemoteConnAllowed.x64=11EEE4
bMultimonAllowed.x64  =11EEE8
ulMaxDebugSessions.x64=11EEF0
bFUSEnabled.x64       =11EEF4

[10.0.21359.1-SLInit]
bInitialized.x64      =11EECC
bServerSku.x64        =11EED0
lMaxUserSessions.x64  =11EED4
bAppServerAllowed.x64 =11EEDC
bRemoteConnAllowed.x64=11EEE4
bMultimonAllowed.x64  =11EEE8
ulMaxDebugSessions.x64=11EEF0
bFUSEnabled.x64       =11EEF4

[10.0.21370.1-SLInit]
bInitialized.x64      =11EECC
bServerSku.x64        =11EED0
lMaxUserSessions.x64  =11EED4
bAppServerAllowed.x64 =11EEDC
bRemoteConnAllowed.x64=11EEE4
bMultimonAllowed.x64  =11EEE8
ulMaxDebugSessions.x64=11EEF0
bFUSEnabled.x64       =11EEF4

[10.0.21376.1-SLInit]
bInitialized.x64      =11EECC
bServerSku.x64        =11EED0
lMaxUserSessions.x64  =11EED4
bAppServerAllowed.x64 =11EEDC
bRemoteConnAllowed.x64=11EEE4
bMultimonAllowed.x64  =11EEE8
ulMaxDebugSessions.x64=11EEF0
bFUSEnabled.x64       =11EEF4

[10.0.21382.1-SLInit]
bInitialized.x64      =11EECC
bServerSku.x64        =11EED0
lMaxUserSessions.x64  =11EED4
bAppServerAllowed.x64 =11EEDC
bRemoteConnAllowed.x64=11EEE4
bMultimonAllowed.x64  =11EEE8
ulMaxDebugSessions.x64=11EEF0
bFUSEnabled.x64       =11EEF4

[10.0.21387.1-SLInit]
bInitialized.x64      =11FECC
bServerSku.x64        =11FED0
lMaxUserSessions.x64  =11FED4
bAppServerAllowed.x64 =11FEDC
bRemoteConnAllowed.x64=11FEE4
bMultimonAllowed.x64  =11FEE8
ulMaxDebugSessions.x64=11FEF0
bFUSEnabled.x64       =11FEF4

[10.0.21390.1-SLInit]
bInitialized.x64      =11FECC
bServerSku.x64        =11FED0
lMaxUserSessions.x64  =11FED4
bAppServerAllowed.x64 =11FEDC
bRemoteConnAllowed.x64=11FEE4
bMultimonAllowed.x64  =11FEE8
ulMaxDebugSessions.x64=11FEF0
bFUSEnabled.x64       =11FEF4

[10.0.21996.1-SLInit]
bInitialized.x64      =11FECC
bServerSku.x64        =11FED0
lMaxUserSessions.x64  =11FED4
bAppServerAllowed.x64 =11FEDC
bRemoteConnAllowed.x64=11FEE4
bMultimonAllowed.x64  =11FEE8
ulMaxDebugSessions.x64=11FEF0
bFUSEnabled.x64       =11FEF4

[10.0.22000.1-SLInit]
bInitialized.x64      =11FECC
bServerSku.x64        =11FED0
lMaxUserSessions.x64  =11FED4
bAppServerAllowed.x64 =11FEDC
bRemoteConnAllowed.x64=11FEE4
bMultimonAllowed.x64  =11FEE8
ulMaxDebugSessions.x64=11FEF0
bFUSEnabled.x64       =11FEF4

[10.0.22000.318-SLInit]
bInitialized.x64      =11FECC
bServerSku.x64        =11FED0
lMaxUserSessions.x64  =11FED4
bAppServerAllowed.x64 =11FEDC
bRemoteConnAllowed.x64=11FEE4
bMultimonAllowed.x64  =11FEE8
ulMaxDebugSessions.x64=11FEF0
bFUSEnabled.x64       =11FEF4

[10.0.22000.466-SLInit]
bInitialized.x64      =11FECC
bServerSku.x64        =11FED0
lMaxUserSessions.x64  =11FED4
bAppServerAllowed.x64 =11FEDC
bRemoteConnAllowed.x64=11FEE4
bMultimonAllowed.x64  =11FEE8
ulMaxDebugSessions.x64=11FEF0
bFUSEnabled.x64       =11FEF4

[10.0.22000.469-SLInit]
bInitialized.x64      =11FECC
bServerSku.x64        =11FED0
lMaxUserSessions.x64  =11FED4
bAppServerAllowed.x64 =11FEDC
bRemoteConnAllowed.x64=11FEE4
bMultimonAllowed.x64  =11FEE8
ulMaxDebugSessions.x64=11FEF0
bFUSEnabled.x64       =11FEF4

[10.0.22000.652-SLInit]
bInitialized.x64      =11FECC
bServerSku.x64        =11FED0
lMaxUserSessions.x64  =11FED4
bAppServerAllowed.x64 =11FEDC
bRemoteConnAllowed.x64=11FEE4
bMultimonAllowed.x64  =11FEE8
ulMaxDebugSessions.x64=11FEF0
bFUSEnabled.x64       =11FEF4

[10.0.22000.653-SLInit]
bInitialized.x64      =11FECC
bServerSku.x64        =11FED0
lMaxUserSessions.x64  =11FED4
bAppServerAllowed.x64 =11FEDC
bRemoteConnAllowed.x64=11FEE4
bMultimonAllowed.x64  =11FEE8
ulMaxDebugSessions.x64=11FEF0
bFUSEnabled.x64       =11FEF4

[10.0.22000.708-SLInit]
bInitialized.x64      =11FECC
bServerSku.x64        =11FED0
lMaxUserSessions.x64  =11FED4
bAppServerAllowed.x64 =11FEDC
bRemoteConnAllowed.x64=11FEE4
bMultimonAllowed.x64  =11FEE8
ulMaxDebugSessions.x64=11FEF0
bFUSEnabled.x64       =11FEF4

[10.0.22449.1000-SLInit]
bInitialized.x64      =11FF0C
bServerSku.x64        =11FF10
lMaxUserSessions.x64  =11FF14
bAppServerAllowed.x64 =11FF1C
bRemoteConnAllowed.x64=11FF24
bMultimonAllowed.x64  =11FF28
ulMaxDebugSessions.x64=11FF30
bFUSEnabled.x64       =11FF34

[10.0.22454.1000-SLInit]
bInitialized.x64      =11FF0C
bServerSku.x64        =11FF10
lMaxUserSessions.x64  =11FF14
bAppServerAllowed.x64 =11FF1C
bRemoteConnAllowed.x64=11FF24
bMultimonAllowed.x64  =11FF28
ulMaxDebugSessions.x64=11FF30
bFUSEnabled.x64       =11FF34

[10.0.22458.1000-SLInit]
bInitialized.x64      =11FF1C
bServerSku.x64        =11FF20
lMaxUserSessions.x64  =11FF24
bAppServerAllowed.x64 =11FF2C
bRemoteConnAllowed.x64=11FF34
bMultimonAllowed.x64  =11FF38
ulMaxDebugSessions.x64=11FF40
bFUSEnabled.x64       =11FF44

[10.0.22463.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22468.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22471.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22478.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22483.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22489.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22494.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22499.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22504.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22509.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22518.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22523.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22526.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22533.1001-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22538.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22543.1000-SLInit]
bInitialized.x64      =121F2C
bServerSku.x64        =121F30
lMaxUserSessions.x64  =121F34
bAppServerAllowed.x64 =121F3C
bRemoteConnAllowed.x64=121F44
bMultimonAllowed.x64  =121F48
ulMaxDebugSessions.x64=121F50
bFUSEnabled.x64       =121F54

[10.0.22557.1-SLInit]
bInitialized.x64      =127F2C
bServerSku.x64        =127F30
lMaxUserSessions.x64  =127F34
bAppServerAllowed.x64 =127F3C
bRemoteConnAllowed.x64=127F44
bMultimonAllowed.x64  =127F48
ulMaxDebugSessions.x64=127F50
bFUSEnabled.x64       =127F54

[10.0.22563.1-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.22567.1-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.22572.1-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.22579.1-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.22581.1-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.22593.1-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.22598.1-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.22610.1-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.22616.1-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.22621.1-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.22621.317-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.22621.436-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.25115.1000-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.25120.1000-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.25126.1000-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.25131.1000-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.25136.1000-SLInit]
bInitialized.x64      =128F2C
bServerSku.x64        =128F30
lMaxUserSessions.x64  =128F34
bAppServerAllowed.x64 =128F3C
bRemoteConnAllowed.x64=128F44
bMultimonAllowed.x64  =128F48
ulMaxDebugSessions.x64=128F50
bFUSEnabled.x64       =128F54

[10.0.25140.1000-SLInit]
bInitialized.x64      =128F4C
bServerSku.x64        =128F50
lMaxUserSessions.x64  =128F54
bAppServerAllowed.x64 =128F5C
bRemoteConnAllowed.x64=128F64
bMultimonAllowed.x64  =128F68
ulMaxDebugSessions.x64=128F70
bFUSEnabled.x64       =128F74

[10.0.25145.1000-SLInit]
bInitialized.x64      =128F4C
bServerSku.x64        =128F50
lMaxUserSessions.x64  =128F54
bAppServerAllowed.x64 =128F5C
bRemoteConnAllowed.x64=128F64
bMultimonAllowed.x64  =128F68
ulMaxDebugSessions.x64=128F70
bFUSEnabled.x64       =128F74

[10.0.25151.1000-SLInit]
bInitialized.x64      =128F4C
bServerSku.x64        =128F50
lMaxUserSessions.x64  =128F54
bAppServerAllowed.x64 =128F5C
bRemoteConnAllowed.x64=128F64
bMultimonAllowed.x64  =128F68
ulMaxDebugSessions.x64=128F70
bFUSEnabled.x64       =128F74

[10.0.25158.1000-SLInit]
bInitialized.x64      =128F4C
bServerSku.x64        =128F50
lMaxUserSessions.x64  =128F54
bAppServerAllowed.x64 =128F5C
bRemoteConnAllowed.x64=128F64
bMultimonAllowed.x64  =128F68
ulMaxDebugSessions.x64=128F70
bFUSEnabled.x64       =128F74

[10.0.25163.1000-SLInit]
bInitialized.x64      =127F4C
bServerSku.x64        =127F50
lMaxUserSessions.x64  =127F54
bAppServerAllowed.x64 =127F5C
bRemoteConnAllowed.x64=127F64
bMultimonAllowed.x64  =127F68
ulMaxDebugSessions.x64=127F70
bFUSEnabled.x64       =127F74

[10.0.25169.1000-SLInit]
bInitialized.x64      =127F4C
bServerSku.x64        =127F50
lMaxUserSessions.x64  =127F54
bAppServerAllowed.x64 =127F5C
bRemoteConnAllowed.x64=127F64
bMultimonAllowed.x64  =127F68
ulMaxDebugSessions.x64=127F70
bFUSEnabled.x64       =127F74

[10.0.25174.1000-SLInit]
bInitialized.x64      =127F4C
bServerSku.x64        =127F50
lMaxUserSessions.x64  =127F54
bAppServerAllowed.x64 =127F5C
bRemoteConnAllowed.x64=127F64
bMultimonAllowed.x64  =127F68
ulMaxDebugSessions.x64=127F70
bFUSEnabled.x64       =127F74
