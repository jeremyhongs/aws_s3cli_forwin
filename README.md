# aws_s3_cli_forwin

- 윈도우 환경에서 CLI를 통해 S3 테스트
- [AWS CLI Install URL](https://docs.aws.amazon.com/ko_kr/cli/latest/userguide/install-cliv2-windows.html)
- [Download latest AWS CLI](https://awscli.amazonaws.com/AWSCLIV2.msi)

### 설치 후
- 윈도우 'cmd'에서 'aws --version' check

### AWS IAM 설정
- CLI로 접근하기 위한 사용자를 생성하기 위함
- 계정 생성 후, 발급되는 CSV 다운받아 활용

### CLI환경에서 S3 사용
> 기본 명령구조는 aws s3 <s3-command> <source-file/path> <destination-file/path>
- 예시 (copy, move, delete)
```
    Copy/Move
       - local to S3 : aws s3 cp|mv <file-name> S3://<bucket-name>/<directory-name>/
       - S3 to local : aws s3 cp|mv S3://<bucket-name>/<directory-name>
    Delete
       aws s3 rm S3://<bucket-name>/<file-name>
```
- 참고 : [S3 CLI 명령어 설명](https://docs.aws.amazon.com/ko_kr/cli/latest/userguide/cli-services-s3-commands.html)
