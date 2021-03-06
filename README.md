# awstools [![Docker Repository on Quay](https://quay.io/repository/broamski/awstools/status "Docker Repository on Quay")](https://quay.io/repository/broamski/awstools)

## Usage
    docker pull quay.io/broamski/awstools
    docker run --rm -it -v ~/.aws:/home/worker/.aws quay.io/broamski/awstools

## Included Tools
```
metaq.py - Query instances by tag data. Returns: instance id, Name tag, private and public IP addresses
    # Query for instances with a certain key
    python metaq.py --query key --key <value_of_key>

    # Query for instances with a certain value
    python metaq.py --query value --value <value_of_value>

    # Query for instances with a specified key/value combination
    python metaq.py --query both --key <some_key> --value <some_value>
ecs\
    task_def_diff.py - Perform a visual diff of Elastic Container Service Task Definitions
cloudwatch\
    cw_logs_tail.py - Tail a CloudWatch Logs log group, similar to your favorite command: tail -f <file>
```
