# Change Log

## Unreleased

- Changelog.md:
  - Created
- Readme.md:
  - Fixed Markdown rule violations.
  - Added missing cmdlets.
  - Updated branch badges for CodeCov.io to point to mainline
    fork.
- Unit Tests:
  - Fixed PS Script Analyzer and added support for reporting on
    warning-level rules. Copied from Microsoft DSC Resource Kit
    test methodology.
- Split the module into lib files to reduce the size of the main
  module.
- Visual Studio Code Workspace settings:
  - Added to ensure style guidelines matched when using VSCode.
- Improved AppVeyor build to get Pester from PSGallery instead
  of Chocolatey so that latest version is used.
- Increased integration test scenarios/stories.
- Added codecov.io support to report on code coverage.
- Moved all functions for continuous integration into `ci` folder.
- Get-VstsEndpointUri Cmdlet:
  - Added function to return the VSTS endpoint URI builder object.
  - Added unit tests.
- Get-VstsQueryStringParametersFromBound Cmdlet:
  - Added function to support additional parameters and queries.
  - Added unit tests.
- New-VstsSession Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Added unit tests.
  - Added parameter sets for VSTS and TFS.
- Invoke-VstsEndpoint Cmdlet:
  - Added documentation.
  - Added support for alternate endpoint names to support VSRM
    API endpoint.
  - Added support for extended query parameters to support
    parameters pre-pended with `$`, such as `top`.
  - Added CmdletBinding and other PowerShell best practice changes.
- Get-VstsAuthorization Cmdlet:
  - Added documentation.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Added unit tests.
- Get-VstsProject Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Added StateFilter parameter for querying on StateFilter.
  - Added Top and Skip parameter for limiting result set.
- Wait-VSTSProject Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Added RetryIntervalSec parameter to support controlling test
    frequency.
  - Added AccountName, User and Token parameters.
  - Added State parameter to enable waiting for a project to enter
    a specific state.
  - Refactored to improve verbose logging and edge case handling.
- New-VSTSProject Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Changed Wait parameter to wait for a project to enter the
    WellFormed state.
- Remove-VSTSProject Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Suppress output of REST API from being placed into pipeline.
- Get-VstsProcess Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Added Id parameter to allow querying a specific Id.
  - Added AccountName, User and Token parameters.
- Get-VstsBuildArtifact Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
- Get-VstsReleaseDefinition Cmdlet:
  - Added cmdlet to get a specific release definitions or all
    release definitions.
- Get-VstsRelease Cmdlet:
  - Added cmdlet to get a list of releases by query or all
    releases.
- New-VstsRelease Cmdlet:
  - Added cmdlet to create a new release.
- Get-VstsCodePolicyConfiguration Cmdlet:
  - BREAKING: Renamed from Get-VstsCodePolicy to match actual purpose.
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Added Top and Skip parameter for limiting result set.
- New-VstsCodePolicyConfiguration Cmdlet:
  - BREAKING: Renamed from New-VstsCodePolicy to match actual purpose.
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
- Get-VstsWorkItem Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Added additional query options to improve work item lookup.
- New-VstsWorkItem Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Fixed bugs that prevented cmdlet from creating work item.
- Test-Guid Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Added unit tests.
  - Changed Input parameter name to Guid because Input is a reserved
    word.
- Get-VstsGitRepository Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Added repository parameter to filter on repository id or name.
  - Unit tests completed.
- New-VstsGitRepository Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
- Remove-VstsGitRepository Cmdlet:
  - Added cmdlet to delete repositories.
  - Unit tests completed.
- Get-VstsBuildTag Cmdlet:
  - Added cmdlet to get build tags from a build or entire project.
- Get-VstsBuildDefinition Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Unit tests completed.
- New-VstsBuildDefinition Cmdlet:
  - Added documentation.
  - Style consistency cleanup.
  - Added CmdletBinding and other PowerShell best practice changes.
  - Unit tests completed.
- Added all cmdlets to manifest creation script.

## 1.0.0.0

- Initial versions
