-> a new autoscaling group

-> 1 launch configuration

-> 2 aws_cloudwatch_metric_alarm, both monitoring the CPUUTILIZATION metric. One alarm for scaling up in case the metric reaches a threshold and another to do the reverse action.

-> 1 aws_autoscaling_policy for each metric alarm

->  1 vpc and settings (subnets, route tables)

-> A SNS topic for notifications pertaining to the ASG actions