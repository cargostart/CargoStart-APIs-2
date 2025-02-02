---
categories: ["SmartCity MXP"]
tags: ["examples"] 
title: "CCIXML Version"
linkTitle: "CCIXML"
date: 2023-12-19
type: docs
weight: 80
description:
---
> BORDERO (NOT SECURED) WITH ULDs

### Manifest
```xml
<AirlineManifest xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <VersionTypeNumber>8</VersionTypeNumber>
  <EndOfMessageCode>LAST </EndOfMessageCode>
  <FlightIDAndPointOfLoading>
    <FlightIdentification>
      <CarrierCode>AA</CarrierCode>
      <FlightNumber>0000A</FlightNumber>
      <DepartureDay>07</DepartureDay>
      <DepartureMonth>DEC</DepartureMonth>
    </FlightIdentification>
    <AirportCode>QVA</AirportCode>
  </FlightIDAndPointOfLoading>
  <DestinationHeader>
    <PART3>
      <PointOfUnloading>
        <AirportCode>MXP</AirportCode>
      </PointOfUnloading>
      <UldLoadedCargo>
        <PART5>
          <ULDDescription>
            <ULDIdentification>
              <ULDType>PMC</ULDType>
              <ULDSerialNumber>25242</ULDSerialNumber>
              <ULDOwnerCode>LX</ULDOwnerCode>
            </ULDIdentification>
            <ULDPositionInformation />
          </ULDDescription>
          <BulkLoadedCargo>
            <PART4>
              <ConsignmentDetail>
                <AirlinePrefix>724</AirlinePrefix>
                <AWBNumber>47177421</AWBNumber>
                <OriginAirportCityCode>SWK</OriginAirportCityCode>
                <DestinationAirportCityCode>LAX</DestinationAirportCityCode>
                <ShipmentDescriptionCode>T</ShipmentDescriptionCode>
                <NumberOfPieces>1</NumberOfPieces>
                <WeightCode>K</WeightCode>
                <Weight>650</Weight>
                <VolumeDetail>
                  <VolumeCode>MC</VolumeCode>
                  <VolumeAmount>0.00</VolumeAmount>
                </VolumeDetail>
                <ManifestDescriptionOfGoods>CONSOL</ManifestDescriptionOfGoods>
              </ConsignmentDetail>
            </PART4>
          </BulkLoadedCargo>
        </PART5>
        <PART5>
          <ULDDescription>
            <ULDIdentification>
              <ULDType>PMC</ULDType>
              <ULDSerialNumber>15019</ULDSerialNumber>
              <ULDOwnerCode>LH</ULDOwnerCode>
            </ULDIdentification>
            <ULDPositionInformation />
          </ULDDescription>
          <BulkLoadedCargo>
            <PART4>
              <ConsignmentDetail>
                <AirlinePrefix>020</AirlinePrefix>
                <AWBNumber>50768524</AWBNumber>
                <OriginAirportCityCode>SWK</OriginAirportCityCode>
                <DestinationAirportCityCode>BKK</DestinationAirportCityCode>
                <ShipmentDescriptionCode>P</ShipmentDescriptionCode>
                <NumberOfPieces>1</NumberOfPieces>
                <WeightCode>K</WeightCode>
                <Weight>9</Weight>
                <VolumeDetail>
                  <VolumeCode>MC</VolumeCode>
                  <VolumeAmount>0.00</VolumeAmount>
                </VolumeDetail>
                <TotalShipmentDescriptionCode>T</TotalShipmentDescriptionCode>
                <TotalNumberOfPieces>2</TotalNumberOfPieces>
                <ManifestDescriptionOfGoods>CONSOL</ManifestDescriptionOfGoods>
              </ConsignmentDetail>
            </PART4>
            <PART4>
              <ConsignmentDetail>
                <AirlinePrefix>020</AirlinePrefix>
                <AWBNumber>48995402</AWBNumber>
                <OriginAirportCityCode>SWK</OriginAirportCityCode>
                <DestinationAirportCityCode>LAX</DestinationAirportCityCode>
                <ShipmentDescriptionCode>T</ShipmentDescriptionCode>
                <NumberOfPieces>6</NumberOfPieces>
                <WeightCode>K</WeightCode>
                <Weight>1561</Weight>
                <VolumeDetail>
                  <VolumeCode>MC</VolumeCode>
                  <VolumeAmount>0.00</VolumeAmount>
                </VolumeDetail>
                <ManifestDescriptionOfGoods>PHARMA NR</ManifestDescriptionOfGoods>
              </ConsignmentDetail>
            </PART4>
          </BulkLoadedCargo>
        </PART5>
        <PART5>
          <ULDDescription>
            <ULDIdentification>
              <ULDType>PMC</ULDType>
              <ULDSerialNumber>20258</ULDSerialNumber>
              <ULDOwnerCode>LX</ULDOwnerCode>
            </ULDIdentification>
            <ULDPositionInformation />
          </ULDDescription>
          <BulkLoadedCargo>
            <PART4>
              <ConsignmentDetail>
                <AirlinePrefix>724</AirlinePrefix>
                <AWBNumber>50764604</AWBNumber>
                <OriginAirportCityCode>SWK</OriginAirportCityCode>
                <DestinationAirportCityCode>YYZ</DestinationAirportCityCode>
                <ShipmentDescriptionCode>T</ShipmentDescriptionCode>
                <NumberOfPieces>1</NumberOfPieces>
                <WeightCode>K</WeightCode>
                <Weight>105</Weight>
                <VolumeDetail>
                  <VolumeCode>MC</VolumeCode>
                  <VolumeAmount>0.00</VolumeAmount>
                </VolumeDetail>
                <ManifestDescriptionOfGoods>CONSOL</ManifestDescriptionOfGoods>
              </ConsignmentDetail>
            </PART4>
            <PART4>
              <ConsignmentDetail>
                <AirlinePrefix>724</AirlinePrefix>
                <AWBNumber>48997115</AWBNumber>
                <OriginAirportCityCode>SWK</OriginAirportCityCode>
                <DestinationAirportCityCode>TLV</DestinationAirportCityCode>
                <ShipmentDescriptionCode>P</ShipmentDescriptionCode>
                <NumberOfPieces>5</NumberOfPieces>
                <WeightCode>K</WeightCode>
                <Weight>19</Weight>
                <VolumeDetail>
                  <VolumeCode>MC</VolumeCode>
                  <VolumeAmount>0.00</VolumeAmount>
                </VolumeDetail>
                <TotalShipmentDescriptionCode>T</TotalShipmentDescriptionCode>
                <TotalNumberOfPieces>10</TotalNumberOfPieces>
                <ManifestDescriptionOfGoods>DRAWING DIES AN</ManifestDescriptionOfGoods>
              </ConsignmentDetail>
            </PART4>
            <PART4>
              <ConsignmentDetail>
                <AirlinePrefix>724</AirlinePrefix>
                <AWBNumber>50718080</AWBNumber>
                <OriginAirportCityCode>SWK</OriginAirportCityCode>
                <DestinationAirportCityCode>YYZ</DestinationAirportCityCode>
                <ShipmentDescriptionCode>T</ShipmentDescriptionCode>
                <NumberOfPieces>1</NumberOfPieces>
                <WeightCode>K</WeightCode>
                <Weight>252.4</Weight>
                <VolumeDetail>
                  <VolumeCode>MC</VolumeCode>
                  <VolumeAmount>0.00</VolumeAmount>
                </VolumeDetail>
                <ManifestDescriptionOfGoods>PERSONAL EFFECT</ManifestDescriptionOfGoods>
              </ConsignmentDetail>
            </PART4>
            <PART4>
              <ConsignmentDetail>
                <AirlinePrefix>724</AirlinePrefix>
                <AWBNumber>50760242</AWBNumber>
                <OriginAirportCityCode>SWK</OriginAirportCityCode>
                <DestinationAirportCityCode>PEK</DestinationAirportCityCode>
                <ShipmentDescriptionCode>T</ShipmentDescriptionCode>
                <NumberOfPieces>3</NumberOfPieces>
                <WeightCode>K</WeightCode>
                <Weight>1346</Weight>
                <VolumeDetail>
                  <VolumeCode>MC</VolumeCode>
                  <VolumeAmount>0.00</VolumeAmount>
                </VolumeDetail>
                <ManifestDescriptionOfGoods>CONSOL</ManifestDescriptionOfGoods>
              </ConsignmentDetail>
            </PART4>
          </BulkLoadedCargo>
        </PART5>
        <PART5>
          <ULDDescription>
            <ULDIdentification>
              <ULDType>PMC</ULDType>
              <ULDSerialNumber>21535</ULDSerialNumber>
              <ULDOwnerCode>AZ</ULDOwnerCode>
            </ULDIdentification>
            <ULDPositionInformation />
          </ULDDescription>
          <BulkLoadedCargo>
            <PART4>
              <ConsignmentDetail>
                <AirlinePrefix>055</AirlinePrefix>
                <AWBNumber>50732080</AWBNumber>
                <OriginAirportCityCode>TRN</OriginAirportCityCode>
                <DestinationAirportCityCode>SFO</DestinationAirportCityCode>
                <ShipmentDescriptionCode>T</ShipmentDescriptionCode>
                <NumberOfPieces>1</NumberOfPieces>
                <WeightCode>K</WeightCode>
                <Weight>762</Weight>
                <VolumeDetail>
                  <VolumeCode>MC</VolumeCode>
                  <VolumeAmount>0.00</VolumeAmount>
                </VolumeDetail>
                <ManifestDescriptionOfGoods>CONSOLIDATED SH</ManifestDescriptionOfGoods>
              </ConsignmentDetail>
              <OtherCustomsInformation>
                <OCI>
                  <CustomsInformationIdentifier>ST</CustomsInformationIdentifier>
                  <SupplementaryCustomsInformation>..H..ALH..H..</SupplementaryCustomsInformation>
                </OCI>
              </OtherCustomsInformation>
            </PART4>
          </BulkLoadedCargo>
        </PART5>
      </UldLoadedCargo>
    </PART3>
  </DestinationHeader>
</AirlineManifest>
```
> Please Note:
> - By default if "..AG.." tag is not present, the sender SmartCityMXP freight forwarder code will be used
> - if "..S.." tag is not present, **the bordero is not secured**. 