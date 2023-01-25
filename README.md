# com.castsoftware.labs.ctl.link
Create links between Mainframe Control Parameters and DB2 Cobol Programs


Changes needs to be done in console configuration files.

Code-scanner-config.xml

        <discoverer extensionId="com.castsoftware.uc.asmzos" dmtId="asmzosfilediscoverer"
                    fileExtensions=".asm;.ASM;.mlc;.MLC;.asmacro;.ASMACRO;" label="ASMZOS"/>
        <discoverer extensionId="com.castsoftware.uc.easytrieve" dmtId="esyzosfilediscoverer"
                    fileExtensions=".ESY;.MAC;.esy;.mac" label="Easy"/>
        <discoverer extensionId="com.castsoftware.labs.ctl.link" dmtId="ctlzosfilediscoverer"
                    fileExtensions=".CTL;.ctl;.ndm;.NDM;" label="CTL"/>


dependencies-matrix.xml

   <technology symbol="ASMZOS" type="language">
        <allow symbol="SQL"/>
    </technology>

    <technology symbol="CTL" type="language">
        <allow symbol="SQL"/>
    </technology>

    <technology symbol="Easy" type="language">
        <allow symbol="SQL"/>
    </technology>
