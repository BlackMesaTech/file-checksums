# SHA file checksums

Get SHA file checksums

## Example usage

```yaml
steps:
  - name: Get checksums
    id: file-checksums
    uses: pavelsaman/file-checksums@v1.0.0
    with:
      file-path: README.md
  - name: Display file checksums
    run: |
      echo ${{ steps.file-checksums.outputs.sha1 }}
      echo ${{ steps.file-checksums.outputs.sha224 }}
      echo ${{ steps.file-checksums.outputs.sha256 }}
      echo ${{ steps.file-checksums.outputs.sha284 }}
      echo ${{ steps.file-checksums.outputs.sha512 }}
```
