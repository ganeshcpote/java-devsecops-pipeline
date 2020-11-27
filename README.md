# DevSecOps Pipeline for Java Projects

## Pipeline Overview
![pipelineImport](/images/pipelineoverview.png)

Following stages are present in current DevSecOps Jenkins Pipeline

1. SCM Checkout
2. Code Build
3. Run JUnit Test
4. Open Task Scanner
5. CheckStyle
6. PMD
7. Duplicate Code
8. FindBugs
9. SpotBugs
10. OWASP Dependecy-Check Vulnerabilities
11. SonarQube Analysis
12. Building Docker Image
13. Deploy Docker Image
14. Anchor Docker Scan
    Configure Anchor : 
    mkdir ~/anchor
    cd ~/anchor
    curl https://docs.anchore.com/current/docs/engine/quickstart/docker-compose.yaml > docker-compose.yaml
    docker-compose up -d
    Jenkins Config :
    ![config](/images/anchor-config.png)

## Type of Reports
![reportsImport](/images/reports.png)

Following section shows individual report and their reporting screenshots
1. Test Result
![reportsImport](/images/testresult.png)

2. PMD Warnings
![reportsImport](/images/pmd-1.png)
![reportsImport](/images/pmd2.png)

3. FingBugs Warnings
![reportsImport](/images/findbugs1.png)
![reportsImport](/images/findbugs2.png)

4. SpotBugs Warnings
![reportsImport](/images/spotbugs1.png)
![reportsImport](/images/spotbugs2.png)

5. Dependecy-Check
![reportsImport](/images/depdency-check.png)

6. Check-Stype Warnings
![reportsImport](/images/check-stype1.png)
![reportsImport](/images/check-stype2.png)

7. CPD Duplications
![reportsImport](/images/cpd1.png)
![reportsImport](/images/cpd2.png)

8. Anchor Report
![reportsImport](/images/anchor1.png)
![reportsImport](/images/anchor2.png)
