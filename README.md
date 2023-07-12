# study-scas

## Requirements on the gNB

[TS 33.501, clause 5.3.2.](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiLlZz21YOAAxUw-DgGHVAZDjIQFnoECBgQAQ&url=https%3A%2F%2Fwww.etsi.org%2Fdeliver%2Fetsi_ts%2F133500_133599%2F133501%2F15.04.00_60%2Fts_133501v150400p.pdf&usg=AOvVaw3176yqNSzVeIECCr6sVaNG&opi=89978449)
### User data and signalling data confidentiality
* The gNB shall support ciphering of user data between the UE and the gNB.
* The gNB shall activate ciphering of user data based on the security policy sent by the SMF.
* The gNB shall support ciphering of RRC-signalling.
* The gNB shall implement the following ciphering algorithms:
  - NEA0, 128-NEA1, 128-NEA2 as defined in Annex D of the present document.
  - Examples....
* The gNB may implement the following ciphering algorithm:
  - 128-NEA3 as defined in Annex D of the present document.
*  Confidentiality protection of user data between the UE and the gNB is optional to use.
*  Confidentiality protection of the RRC-signalling is optional to use.
*  Confidentiality protection should be used whenever regulations permit.

### User data and signalling data integrity
* The gNB shall support integrity protection and replay protection of user data between the UE and the gNB.
* The gNB shall activate integrity protection of user data based on the security policy sent by the SMF.
* The gNB shall support integrity protection and replay protection of RRC-signalling.
* The gNB shall support the following integrity protection algorithms:
   - NIA0, 128-NIA1, 128-NIA2 as defined in Annex D of the present document.
* The gNB may support the following integrity protection algorithm:
   - 128-NIA3 as defined in Annex D of the present document.
* Integrity protection of the user data between the UE and the gNB is optional to use, and shall not use NIA0.


# 4.2.2.1.10 Ciphering of user data based on the security policy sent by the SMF

## Requirements
* _Requirement Name_: Replay protection of RRC-signalling.
* _Requirement Reference_: TS 33.501 [2], clause 5.3.3
* _Requirement Description_: "The gNB shall support integrity protection and replay protection of RRC-signalling " as
specified in TS 33.501 [2], clause 5.3.3.
* _Threat References_: TR 33.926 [5], clause D.2.2.2 – Control plane data integrity protection.

  _D.2.2.8 Security Policy Enforcement_
   - _Threat name: Security Policy Enforcement._
 - _Threat Category: Tampering data, Information Disclosure._
 - _Threat Description: If gNB does not follow the security based on security policy provided by SMF, this can lead_
 - _to no security or reduced security provided to the UE user plane, (e.g. not applying integrity protection when it is_
 - _required to do so), etc.Threatened Asset: Sufficient Processing Capability, User plane data._



# 4.2.2.1.11 Integrity of user data based on the security policy sent by the SMF
